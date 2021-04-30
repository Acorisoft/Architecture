# 关系元数据

## 关系的可见性（设定、元数据字段）

* 公开
* 私密
* 秘密

## 反应（设定字段）

* 厌恶
* 疏远
* 躲避
* 害羞
* 尴尬
* 保持距离
* 陌生
* 正常
* 靠近
* 亲密
* 喜欢
* 崇拜

## 关系的类型（设定、元数据字段）

* 人际类型
* 家庭类型
* 亲密关系

## 是否为性伴侣（设定、元数据字段）

* 是
* 否

## 死亡状态（设定、元数据字段）

* 生存
* 死亡
* 未知

## 肢体接触程度（设定、元数据字段）

* 一垒
* 二垒
* 三垒
* 本垒（如果设置为性伴侣，直接设置为本垒）

# 人际关系

## 人际关系类型

* 朋友类
    * 网友
    * 亲友
    * 朋友
    * 陌生人
    * 损友
    * 挚友
    * 死党
* 学校类
    * 老师
    * 校友
    * 同学
    * 舍友
    * 师傅
    * 徒弟
    * 学生
* 社会类
    * 同事
    * 雇主
    * 雇佣
    * 看护
    * 保镖
    * 
* 特殊关系类
    * 崇拜

## 人际关系的历程

* 脆弱
* 破裂
* 舒适
* 柏拉图式
* 麻木
* 危险
* 稳固
* 紧绷
* 动荡
* 升温
* 热烈

## 虐待关系

* 肢体暴力
* 言语暴力
* 精神暴力

## 人际关系状态

* 喜欢
* 讨厌
* 崇拜
* 正常

# 家庭关系

## 家庭关系类型

* 丈夫
* 妻子
* 父亲
* 母亲
* 儿子
* 女儿
* 姐妹
* 兄弟

## 家庭关系的血缘关系

* 直系
* 旁系
* 支系

## 家庭关系的辈分

* 祖辈
* 父辈
* 儿辈
* 孙辈

## 家庭关系的状态

* 前任
* 现任
* 继任

## 自定义关系名

## 同居状态

* 同居
* 分居

# 亲密关系

## 亲密关系的类型

* 异性
* 同性

## 亲密关系的状态

* 追求
* 交往
* 订婚
* 分手
* 饲养
* 暧昧

## 对待亲密关系的态度

* 随意
* 认真
* 专一

## 亲密关系的情况

* 踯躅
* 脆弱
* 破裂
* 舒适
* 柏拉图式
* 稳固
* 紧绷
* 升温
* 热烈

## 亲密关系的反馈

* 接受
* 拒绝
* 不表态

# 关系元数据的描述

# 关系元数据的伪代码

``` C#
public interface IRelationshipMetadata
{
    RelationshipVisibility Visibility { get; set; }
    MeetReaction Reaction { get; set; }
    RelationshipType RelationshipType { get; set; }    
    PhysicalTouchProgress Progress { get; set; }
    bool IsSexPartner { get; set; }
    AliveState Death { get; set; }
    bool IsClosed { get; set;}
}

public interface IInterpersonalRelationship : IRelationshipMetadata
{
    InterpersonalRelation Relationship { get; set; }
    InterpersonalIntimacy Intimacy { get; set; }
    AbusiveRelationship Abusive { get; set; }
}

public interface IFamilyRelationship : IRelationshipMetadata
{
    FamilyRelationship Relationship { get; set; }
    Kinship Kinship { get; set; }
    Generation Generation { get; set; }
	FamilyRelationshipStatus Status { get; set; }
    string CustomName { get; set; }
    bool Cohabitation { get; set; }
}

public interface IIntimateRelationship : IRelationshipMetadata
{
    IntimateRelationship Relationship { get; set; }
    IntimateRelationshipStatus Status { get; set; }
    IntimateRelationshipAttitude Attitude { get; set; }
    IntimateRelationshipDescription Description { get; set; }
    IntimateRelationshipFeedback Feedback { get; set; }
}

```


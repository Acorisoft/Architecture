# 人物关系

## 设计难点

1. 复合人物关系

    > 我们拟使用数组的方式来实现复合人物关系

2. 中外各方的人物关系称谓不一致

    > 我们拟用原语的方式，来实现统一的称谓

3. 多元关系



## 人物关系的状态

人物关系的状态其实指的是当前人物关系的实际情况，我们关注的是这个人物当前是过去时还是现在时。

* Former(前、以前的)
* Incumbent (现任)
* Succession（继任，继，后）

【元数据字段】【模组字段】

## 人物关系的现状

人物关系的状态指的是当前人物关系的实际状态，关注的是人物关系当前是过去时还是现在时，而现状指的是人物关系目前处于什么模式。关注的是关系现在的进展。

* 怀念（前任）【又复合的可能】
* 断念（前任）【无符合的可能】
* 路人（前任）【一般朋友】
* 亲密（前任，现任，继任）【聊得还是很可以的】
* 破裂（前任，现任，继任）
* 保持距离（前任，现任，继任）
* 危险（现任，继任）
* 紧绷（现任，继任）
* 动荡（现任，继任）
* 脆弱（现任，继任）
* 易碎（现任，继任）
* 稳固（现任，继任）
* 麻木（现任，继任）
* 柏拉图式（前任，现任，继任）
* 舒服（现任，继任）
* 升温（现任，继任）
* 热烈（现任，继任）
* 狂热（现任，继任）

【模组字段】

## 人物关系的特殊标记

性伴侣关系、关系的认可标记（未回复，不明确，双方接受，单方拒绝，单方接受）、虐待标志（肢体虐待，言语虐待，精神虐待，性虐待）、性侵标志（是、否）

## 人物关系的类型

* 亲密关系
    * 闺蜜
    * 知己
    * 朋友
    * 死党
    * 损友
    * 挚友
    * 陌路人
    * 情侣
    * CP
    * 情敌
    * 初恋
    * 追求者
    * 爱慕
    * 伙伴
    * 同好
    * 亲友
    * 基友
* 家庭关系
    * 原生家庭
        * 祖父
        * 祖母
        * 外祖母
        * 外祖父
        * 父亲
        * 母亲
        * 姐姐
        * 妹妹
        * 弟弟
        * 哥哥
        * 儿子
        * 女儿
        * 孙子
        * 孙女
        * 外孙女
        * 外孙子
        * 女婿
        * 儿媳
        * 丈夫
        * 妻子
        * 妾室
    * 阶梯家庭
        * 继父
        * 继母
        * 继姐
        * 继兄
        * 继弟
        * 继妹
        * 看护
        * 领养
    * 复杂家庭
        * 义父
        * 义母
        * 义兄
        * 义弟
        * 义姐
        * 义妹
    * 旁系
        * 伯父
        * 伯母
        * 伯伯
        * 婶婶
        * 叔父
        * 叔母
        * 叔叔
        * 阿姨
        * 舅舅
        * 舅妈
        * 姑姑
        * 姑爷
        * 堂哥
        * 堂弟
        * 堂姐
        * 堂妹
        * 表哥
        * 表姐
        * 表妹
        * 表弟
        * 宗族
        * 远亲
* 人际关系
    * 学校
        * 学生
        * 老师
        * 徒弟
        * 师傅
        * 校友
        * 同学
        * 舍友
        * 学长
        * 学弟
        * 学妹
        * 学姐
* 社会关系
    * 室友
    * 同事
    * 雇主
    * 雇佣
    * 主人
    * 仆人
    * 奴隶
    * 管家
    * 前辈
    * 晚辈
    * 陌生人
    * 邻居
    * 崇拜
    * 偶像
    * 跟班
    * 领袖
    * 随从
    * 敌人
    * 同门
    * 同道
    * 饲养
    * 情人

【元数据字段】【模组字段】

## 人物关系的多元性

【模组字段】

## 肢体接触程度

* 一垒
* 二垒
* 三垒
* 本垒（如果设置为性伴侣，直接设置为本垒）

【元数据字段】【模组字段】

## 人物关系（这里的内容均使用拼音标记）

* 家庭关系
* 社交关系
* 亲密关系
* 人际关系
* 多元关系

【元数据字段】【模组字段】

## 关系的可见性

* 公开
* 私密
* 秘密

【元数据字段】【模组字段】

# 人物关系图生成

人物关系图的生成，需要考虑使用图数据结构。人物是节点，关系是边。

## 渲染层

### 渲染节点

### 渲染边

## 数据层
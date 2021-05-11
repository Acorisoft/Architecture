# 开发者专栏

## 创作的状态

概念时（Concepts-Time）、原型时（Prototype-Time）、设计时（Design-Time）、呈现时（Presentation-Time）。

## 人物设定的概念时

在人物设定的概念态中我们需要使用关键字来实现对概念的描述。概念时所产生的的内容是一种可以替换的键值对的数据。

| 编号 |                      内容                      |                             备注                             |
| :--: | :--------------------------------------------: | :----------------------------------------------------------: |
| 01xx |         用户挑选符合该角色性格的关键字         | 用来挑选符合该角色性格的关键字，这个大类包括但不限于性格。因为性格只是一些文字，我们无法通过单一的性格特征来描述一个人的完整特征。 |
| 02xx |         用户挑选符合该角色外观的关键字         | 通过挑选符合该角色外观上的关键字，来进一步描述这个角色。进而让我们对这个角色的了解更加立体。 |
| 03xx | 用户挑选符合该角色剧情上的定位以及作用的关键字 | 通过挑选符合该角色在剧情上的定位于作用的关键字，来还原这个角色在剧情上的表现，让我们对这个角色的了解更加立体。 |
| 04xx |       用户通过挑选符合该角色癖好的关键字       | 通过挑选符合该角色在癖好上的关键字，来进一步还原角色在行为上的表现。 |
| 05xx |    用户通过挑选符合该角色成长的主题的关键字    |  通过挑选符合该角色在成长主题上的关键字，来进一步还原角色。  |

## 概念时复合数据

概念时数据包括了复合数据、单选数据和自定义数据。其中复合数据我们使用枚举来实现，所有枚举都转成int类型，在通过int类型进行选择

``` C#
public class BasicConceptViewModel
{
    public AcgMoeAppearance Acg{
        get;
        set;
    }
    
    public bool BlackStraightHair{
        get => Acg.HasFlag(AcgMoeAppearance.BlackStraightHair);
        set{
            Acg = ToggleFlag(value, AcgMoeAppearance.BlackStraightHair);
        }
    }
}

/*
	IsKindness = true IsKindness = 0100000 Source = 0001111 Result = 0101111 Operation = Xor Target
	IsKindness = false IsKidness = 0100000 Source = 0001111 Result = 0001111 Operation = ((Not Target) And Source)
*/
```





## 概念时数据样例

``` JSON
{ ID = "MOC-0101", Message = "成长" }
{ ID = "MOC-0101", Data = 2 }
{ ID = "MOC-0101", Data = 6 }
```






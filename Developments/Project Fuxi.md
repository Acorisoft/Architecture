# Project Fuxi

`Project Fuxi` 是研究如何使用.NET + XAML实现模组化的工程项目。我们的项目因为需要实现用户自定义模组的功能，因此我们需要一种机制来帮助我们完成自定义模组。

## 计划步骤

* 实现 DSL 语言
* 实现 DSL to ViewModel
* 实现 ViewModel 视图自动生成。
* 使用MEF实现自动扫描

## 需要考虑的地方

* 如果在DSL中我们需要数据库中的类型，该怎么办？
* 
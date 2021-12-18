# 单向数据流

> 原文:[https://www.geeksforgeeks.org/unidirectional-data-flow/](https://www.geeksforgeeks.org/unidirectional-data-flow/)

单向数据流是一种主要在函数式反应式编程中发现的技术。它也被称为单向数据流，这意味着数据只有一种，而且只有一种方式可以传输到应用程序的其他部分。本质上，这意味着子组件不能更新来自父组件的数据。在 React 中，来自父母的数据被称为**道具**。Angular 利用双向绑定，其中数据流在两个方向上发生。React 不支持双向绑定，以确保遵循干净的数据流架构。这种方法的主要好处是数据在应用程序中单向流动，让您可以更好地控制它。
就反应而言，它的意思是:

*   状态被传递给视图和子组件
*   操作由视图触发
*   操作可以更新状态
*   状态更改被传递给视图和子组件

**注意:**视图是应用程序状态的结果。行动发生时状态会改变。当动作发生时，状态会更新。

单向数据绑定为我们提供了一些关键优势。比如:

*   更容易调试，因为我们知道什么数据来自哪里。
*   更不容易出错，因为我们可以更好地控制数据。
*   效率更高，因为库知道系统每个部分的边界。

在“反应”中，状态总是由一个组件拥有。此状态所做的任何更改只能影响其下的组件，即其子组件。更改组件的状态永远不会影响其父组件或同级组件，只会影响子组件。这是状态经常在组件树中向上移动的主要原因，以便它可以在需要访问它的组件之间共享。
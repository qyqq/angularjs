
### 通过这个例子来初步了解angularjs使用模式
1. angular通过在HTML模板中的ng标记来识别结构DOM层级实现数据绑定，渲染工作

2. 在 js 代码中做了一些数据的操作，事件的绑定定义等。这样，数据的变化就会和页面中的 DOM 表现联系起来，即“双向绑定”。通过“数据变化”这个事件实现。

    利用angular.bootstrap(document.documentElement)驱动整个页面，实现可控大小方块

3. 使用 angular.bootstrap 来显示地做初始化工具，参数指明了根节点，装载的模块（可以是多个模块）。

问题：

对于实现数据驱动用这么一句不是更简单

angular.bootstrap(document.documentElement);

为什么又定义ng-app呢？

var app = angular.module('Demo', [], angular.noop);
angular.bootstrap(document, ['Demo']);

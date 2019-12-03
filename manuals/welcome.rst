========
欢迎使用
========

FizeView 是一个支持各种引擎的视图库。

FizeView 没有再新建一个视图语法，它认为没有这个必要！

世面已经有那么多性能不错，满足各类需求的视图框架了，为什么我们还需要 FizeView ？

因为 FizeView 允许你使用任意的视图引擎，但是又使用相同的视图接口，这样的好处很明显：你可以随意选择自己擅长的视图引擎来编写前端代码。

FizeView 有非常完善的参考文档，且其功能追求简洁明了，相信您会喜欢上这样的视图库。


处理器支持
==========

目前 FizeView 已支持的模板视图引擎处理器如下：

-  :doc:`Blade </configs/blade>` : Laravel 提供的一个简单而又强大的模板引擎。
-  :doc:`Php </configs/php>` : PHP 原生模板引擎 。
-  :doc:`Smarty </configs/smarty>` : 一个历史悠久，经久耐用的模板引擎。
-  :doc:`Think </configs/think>` : 即 ThinkTemplate ，ThinkPHP 的内置模板引擎。
-  :doc:`Twig </configs/twig>` : 一个流行、严谨的模板引擎，多个 IDE 都对 Twig 进行高亮支持。


入门三部曲
==========

1.配置参数
----------

根据 :doc:`参数配置 </configs/index>` 进行FizeView 配置。

2.设置默认模板引擎或者设置新模板引擎
----------------------------

使用 `new View($handler, $config);`进行默认模板引擎设置，或者 `View::getInstance($handler, $config)` 方法获取新模板引擎实例

3.进行模板编写即其他操作
----------------

FizeView 简化了模板的操作，日常您使用的方法如下。

- `View::engine()` : 获取底部引擎对象。
- `View::path()` : 设置模板路径。
- `View::assign()` : 变量赋值。
- `View::render()` : 返回渲染内容。
- `View::display()` : 显示渲染内容。


入门示例
========

.. code-block:: php

	use fize\view\View;

	$config = [
		'path'   => '../view',
		'cache' => '../runtime',
		'debug'  => true
	];
	new View('Twig', $config);  //使用 twig 引擎

	$assigns = ['data' => ['name' => 'evai', 'mobile' => 12345678910]];

	View::display('index', $assigns);
		


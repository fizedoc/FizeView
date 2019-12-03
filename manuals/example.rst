========
代码示例
========

.. code-block:: php

	use fize\view\View;

	$config = [
		'view'   => '../view',
		'cache'  => '../runtime',
		'debug'  => true
	];
	$view = View::getInstance('Twig', $config);  // 使用 Twig 引擎

	$assigns = ['data' => ['name' => 'evai', 'mobile' => 12345678910]];

	$view->display('index', $assigns);

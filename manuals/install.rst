========
安装说明
========

FizeView 的环境要求如下：

-  "php": ">=5.4.0" ， 很多视图引擎要求 PHP7 ，所以还是推荐使用 PHP7 以上版本。
-  如果使用 Blade 引擎，请 composer 安装 `illuminate/view` 。
-  如果使用 Smarty 引擎，请 composer 安装 `smarty/smarty` 。
-  如果使用 Think 引擎，请 composer 安装 `topthink/think-template` 。
-  如果使用 Twig 引擎，请 composer 安装 `twig/twig` 。

使用Composer安装
================

FizeView 支持使用 `Composer <https://www.phpcomposer.com/>`_ 安装，也是唯一官方推荐的安装方法。

.. note::

   如果您尚未安装 composer ，请参考 `安装 composer <https://docs.phpcomposer.com/00-intro.html>`_ 。
   
   使用 `阿里云镜像 <https://developer.aliyun.com/composer>`_ 以提高下载速度及稳定性。


在命令行下面，切换到您的项目根目录下面并执行下面的命令：

.. code-block:: bash

  composer require fize/view

根据需要，选择 FizeView 处理器。使用 composer 下载依赖或者开启相应扩展。
  
好了！您现在可以开始使用 FizeView 了，就是这么简单！~

.. note::

   Fize 项目(包括所有子项目)严格遵守 `语义化版本 <https://semver.org/lang/zh-CN/spec/v2.0.0.html>`_ ，您可以放心大胆的使用。
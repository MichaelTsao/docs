简述
=====

.. _有什么用:

有什么用
------------

easy库基于Tornado和Peewee，通过配置完成CRUD接口搭建。包括如下能力：

 - 数据校验
 - 常规的增删改查、导入导出的逻辑

引入项目
------------
通过git submodule模式可以引入easy库到项目中

.. code-block:: console

    $ git submodule add git@git.hundun.cn:caoxiang/easy.git

控制层
----------------

控制层基于Tornado的RequestHandler。封装了如下逻辑：

 - 可配置的RESTful API 接口
 - 支持跨域
 - 同时支持 Content-Type 为 form 和 json 的格式
 - 鉴权入口
 - 集成了sentry的配置

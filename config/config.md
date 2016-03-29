# 配置文件
配置文件遵循TP的加载顺序，后加载的会覆盖之前加载的配置。

加载顺序：


> 惯例配置->应用配置->模式配置->调试配置->状态配置->模块配置->扩展配置->动态配置


本例中如下：

> tp惯例配置->data/conf/global.php->data/conf/version.php->Common/Conf/config.php->data/conf/db(.default).php->data/conf/config(.default).php->app/MODULE_NAME/conf/config.php



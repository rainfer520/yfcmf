# 全局配置
路径：
> data/conf/global.php


```
//检测php版本
if (version_compare(PHP_VERSION, '5.3.0', '<')) {
    die ('require PHP > 5.3.0 !');
}
//定义HTTP_HOST域名
define ('HTTP_HOST', strtolower(isset ($_SERVER ['HTTP_HOST']) ? $_SERVER ['HTTP_HOST'] : 'unknown'));
//如果存在调试锁文件或者不存在安装锁文件,则设置为开启调试模式 数据库调试模式
if (file_exists(YFCONF_PATH . 'debug.lock') || !file_exists(YFCONF_PATH . 'install.lock')) {
    define ('APP_DEBUG', true);
    define ('DB_DEBUG', true);
} else {
    define ('APP_DEBUG', false);
    define ('DB_DEBUG', false);
}
//存在版本文件就加载
(!file_exists($file = YFCONF_PATH . 'version.php')) && exit('Missing ' . YFCONF_PATH . 'version.php');
include $file;
```

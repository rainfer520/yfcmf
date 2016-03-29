# 数据库配置
路径：
> data/conf/db.php(如果不存在，则读取db.default.php)

```
return array (
  'DB_TYPE' => 'mysql',
  'DB_HOST' => 'localhost',
  'DB_PORT' => '3306',
  'DB_NAME' => 'yfcmf',//数据库名
  'DB_USER' => 'root',//数据库用户名
  'DB_PWD' => '',//数据库密码
  'DB_PREFIX' => 'yf_',//数据库前缀
);
```

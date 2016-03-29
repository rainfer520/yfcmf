# 项目设置
路径：data/conf/config.default.php(此设置为项目的默认设置）
```
return array(
    'SHOW_PAGE_TRACE' => APP_DEBUG ? true : false,//是否显示page_trace
    'DB_DEBUG' => DB_DEBUG ? true : false,
	//设置模板相关路径
    'TMPL_PARSE_STRING' => array(
        '__PUBLIC__' => __ROOT__ . '/themes/public',
        '__DATA__' => __ROOT__ . '/data',
		'__UPLOAD__' => __ROOT__ . '/data/upload',
		'__AVATAR__' => __ROOT__ . '/data/upload/image/avatar',
        '__STATIC_ROOT__' => __ROOT__,
        '__JS_SUFFIX__' => (APP_DEBUG ? '.src.js' : '.js'),
    ),
    'APP_SUB_DOMAIN_DEPLOY' => 1,
    'APP_SUB_DOMAIN_RULES' => array(
        //'domain1.com' => 'Home',
        //'domain2.com' => 'Home'
    ),
    'UPLOAD_TEMP_DIR' => DATA_PATH,
    'UPLOADPATH'=>__ROOT__ . '/data/upload',//上传路径
);
```

路径：
> data/conf/config.php(此设置为后台设置）


```
return array (
  'APP_SUB_DOMAIN_RULES' => 
  array (
    'localhost' => 'Home',
	'www.rainfer.cn' => 'Home',
  ),
  'ADMIN_SCRIPT' => 'admin.php',
  'URL_MODEL' => 3,
);
```

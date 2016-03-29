# 公共配置
路径：
> app/Common/Conf/config.php


```
$cfg = array(
	/*URL设置*/
	'URL_CASE_INSENSITIVE'  => true,   // 默认false 表示URL区分大小写 true则表示不区分大小写
	'URL_MODEL'             => 3,       // URL访问模式,可选参数0、1、2、3,代表以下四种模式：
	'URL_PATHINFO_DEPR'     => '/',	// PATHINFO模式下，各参数之间的分割符号
	'URL_HTML_SUFFIX'       => '',  // URL伪静态后缀设置
	/*日志设置*/
    'LOG_TYPE' => 'File',
    'LOG_RECORD' => true,
    'LOG_EXCEPTION_RECORD' => true,
    'LOG_LEVEL' => 'EMERG,ALERT,CRIT,ERR,WARN,NOTICE',
    /*多语言设置*/
    'LANG_SWITCH_ON' => true,
    'LANG_AUTO_DETECT' => true,
    'LANG_LIST' => 'zh-cn',
    'VAR_LANGUAGE' => 'l',
	/*页面错误 成功设置*/
    'ERROR_MESSAGE' => '页面错误',
    'TMPL_ACTION_ERROR' => __ROOT__ . '/themes/public/dispatch_jump.html',
    'TMPL_ACTION_SUCCESS' => __ROOT__ . '/themes/public/dispatch_jump.html',
    'TMPL_EXCEPTION_FILE' => __ROOT__ . '/themes/public/think_exception.html',
	/*模板风格*/
	'TMPL_PATH'=>'./themes/',
	'DEFAULT_THEME' => 'default',
	'TMPL_DETECT_THEME'     =>  true,       // 自动侦测模板主题
	'TMPL_TEMPLATE_SUFFIX'  =>  '.html',     // 默认模板文件后缀
	/*性能优化*/
	'OUTPUT_ENCODE'			=>true,// 页面压缩输出
	'HTML_CACHE_ON'         =>    false, // 开启静态缓存
	'HTML_CACHE_TIME'       =>    60,   // 全局静态缓存有效期（秒）
	'HTML_FILE_SUFFIX'      =>    '.html', // 设置静态缓存文件后缀
	/*COOKIE SESSION*/
    'COOKIE_HTTPONLY' => true,
    'SESSION_OPTIONS' => array(
        'name' => 'yf_sid'
    ),
	/*缓存*/
    'DATA_CACHE_SUBDIR' => true,//使用子目录缓存
    'DATA_PATH_LEVEL' => 4,//缓存级别
);
```

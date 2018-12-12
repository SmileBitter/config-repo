# config-repo 存放各模块配置文件，springcloud config 启动的时候默认会将配置文件从git上下载放在用户临时目录下缓存
#配置文件映射：
/{application}/{profile}[/{label}]
/{application}-{profile}.yml
/{label}/{application}-{profile}.yml
/{application}-{profile}.properties
/{label}/{application}-{profile}.properties
#其中application是应用名，也可以理解成git上面的文件名，profile指的是对应激活的环境
#名，例如dev、test、prod等，label指的是git的分支，如果不写，默认的分支为master。

# BroadcastTest
*2021-3-31*
安卓8.0版本之后无法使用intent8.0后广播在AndroidManifest.xml中注册后发送intent是接收不到广播了，
看了一下原因，好像是8.0为了管理系统和节约电量特别针对广播和服务发送intent的方式启动做出的改变，也就是说广播和服务不能随意收intent了，
要对广播和服务更精确的指向，所以在创建intent的时候，我们需要指定我们的广播和服务的包名加类名，为的就是精确

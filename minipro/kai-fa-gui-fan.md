# 开发规范

1、按照文件目录结构，严格执行，不要出现冗余文件，代码，要知道小程序的大小是有限的~~~

2、关于数据处理，根据wxs的官方文档，wxs在ios上会比js快2~20倍，在安卓上就无差异。

但由于wxs不能调用小程序的api，也不能作为事件回调，所以我们尽量在通过接口，拿到数据之后的脚本处理，尽量都交给wxs来处

理，由此来让我们的小程序运行得更快。

3、尽量以小程序原生组件为主去开发。

4、开发时，通过api获取信息的方法，除非必要的前置数据，可以使用同步获取，不然全部都采用异步的方式去获取，提高运行效率。


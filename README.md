authority
=========

## 一、什么是Struts2
* Struts 2以WebWork优秀的设计思想为核心，吸收了Struts 1的部分优点，建立了一个兼容WebWork和Struts 1的MVC框架
* Struts 2的目标是希望可以让原来使用Struts 1、WebWork的开发人员，都可以平稳过渡到使用Struts 2框架

## 二、Struts1和Struts2的区别和对比
* struts1于struts2的区别从显示的页面标签上来说，struts1使用的是JSTL标签。
* struts2也使用了JSTL标签，但是它又引入了ognl。 
* struts1对于请求是单例模式的，虽然是线程安全的，但是却影响了性能和action的其他功能的增加
* struts2是每一个请求产生一个实例，没有线程安全的问题，也不会存在性能和垃圾回收的问题。 
* struts1过于依赖servlet API，在所有的执行方法中都要通过参数传入。
* struts2对其进行了解耦， 
* struts1要继承一个抽象基类，再重写execute方法。
* struts2不强制你，可以根据你要使用到的来继承或者实现 
* struts1由于过于依赖servlet API，所以对它进行测试的时候存在着很大的问题。
* struts2解耦了，还可以通过初始化，方法调用等来进行测试 
* struts1要通过ActionFrom类来进行数据交换，还要将它放入pojo送到后台与数据库交互，struts2不用那么复杂，直接在action里定义属性，或者配置好驱动类。 
* struts1验证只有String型的struts2因为有ognl标签，所有很多基本类型以及自己定义的对象都可以验证。


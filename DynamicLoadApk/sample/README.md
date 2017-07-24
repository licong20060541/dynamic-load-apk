# 参考github此工程根目录下的ReadMe.md和Android Studio.md

支持3种plugin对host的调用模式：
（1）无调用（但仍然可以用反射调用）。
（2）部分调用，host可公开部分接口供plugin调用。 这前两种模式适用于plugin开发者无法获得host代码的情况。
（3）完全调用，plugin可以完全调用host内容。这种模式适用于plugin开发者能获得host代码的情况。


#关于sample
这个目录包含了DL架构的sample，目前共有两个：main和depend_on_interface

##main
演示了DL的所有基本功能，建议刚接触DL架构的朋友先看这个sample。
共包含一个Host和两个Plugin。
其中Plugin-A是主要的Plugin，建议先看这个。
Plugin-B使用了前面介绍的第三种开发模式。

##depend_on_interface
这个sample演示了第二种开发模式，通过预装先定的接口（放在doi-common里），可以实现Plugin访问宿主。




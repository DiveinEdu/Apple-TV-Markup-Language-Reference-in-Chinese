# Apple-TV-Markup-Language-Reference-in-Chinese
苹果官方《Apple TV标记语言参考手册》中文翻译版
英文原版：[《Apple TV Markup Language Reference》](https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/index.html#//apple_ref/doc/uid/TP40015064)

本翻译没有获得**苹果公司**的授权，纯属学习爱好。

####欢迎大家帮忙翻译校正或者提供更好的Apple TV开发资料。
####交流群：85157830（AppleTV开发梦工厂）
####问答网站：[潜心俱乐部](http://divein.club)

##致谢
####翻译（按加入时间排序）
- [戴维营教育](http://v.diveinedu.com)
- [AndyLiao8](https://github.com/AndyLiao8)
- [Cheetah.Kiong](https://github.com/wuqiong)
- [wcrane](https://github.com/wcrane)

##在线阅读
本文档使用[Gitbook](http://diveinedu.gitbooks.io/apple-tv-markup-language-reference-in-chinese/)制作，可以直接在线阅读或者导出PDF、EPUB等格式。

####关于 TVML(电视标记语言)

#####概念
######可以使用TVML创建分离的页面在客户端app中，在客户端的每一个页都都用TVML实现，通过模去描述我们想去实现的的一引起元素和安一个布局。每个元素都是为了显示一些信息能过指定的方式，比如，苹果息提供的加载的模板（loading Template）,显示一个简要的信息告诉用户发生了什么事。Rating Template显示一个等级信息，这里还有更多的信息<a href="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/TextboxTemplate.html#//apple_ref/doc/uid/TP40015064-CH2-SW8">关于模板</a>. 当然你可以用一个简单的模板去显示一个页面的信息，也可以在同一个页面里用多个模板去描述你想要显示的信息。
#####你可以能过javascript去控制客户揣的App,javascript文件需要去加载TVML页面，响应用户的输入，更多的信息可以参考<a href="https://developer.apple.com/library/prerelease/tvos/documentation/TVMLJS/Reference/TVJSFrameworkReference/index.html#//apple_ref/doc/uid/TP40016076">TVJS Framework Reference.</a>
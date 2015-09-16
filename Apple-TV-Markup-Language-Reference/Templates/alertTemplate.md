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

###警告模板（alertTemplate）
#####使用警告模板去显示一些重要信息，比如在执行某个操作之前用alertTemplate弹出信息，其中包括问题的描述和按钮，因此需要用户去确认。图2-1，显示一个基本的alertTemplate的布局。

####2-1 警告模板
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/ATV_temps_alert_2x.png" width="678" height="426" >

alertTemplate 主要的元素
#####列表2-1 用TVML格式列出了主要的元素。表格2-1也对这些元素提供了描述

#####列表2-1
<ol class="code-lines">
            <li><code class="code-voice">&lt;alertTemplate&gt;</code></li>
            <li><code class="code-voice">   &lt;title&gt;…&lt;/title&gt;</code></li>
            <li><code class="code-voice">   &lt;description&gt;…&lt;/description&gt;</code></li>
            <li><code class="code-voice">   &lt;button&gt;</code></li>
            <li><code class="code-voice">      &lt;text&gt;…&lt;/text&gt;</code></li>
            <li><code class="code-voice">   &lt;/button&gt;</code></li>
            <li><code class="code-voice">   &lt;text&gt;…&lt;/text&gt;</code></li>
            <li><code class="code-voice">&lt;/alertTemplate&gt;</code></li>
        </ol>
        
#####表格2-1 alertTemplate 的元素的描述：
<table class="graybox" border="0" cellspacing="0" cellpadding="5">
    <thead>
        <tr>
            <th scope="col" class="TableHeading_TableRow_TableCell"><p class="para">
  元素名称
</p></th>
            <th scope="col" class="TableHeading_TableRow_TableCell"><p class="para">
  描述
</p></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW18" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_39&quot;;return this.s_oc?this.s_oc(e):true">button</a></code>
</p></td>
            <td><p class="para">
            按钮，一般它允许用户去关掉当前的alert,或者打开另一个模板页面，按钮元素中有一个文本元素，用来显示按钮的名字
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW8" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_40&quot;;return this.s_oc?this.s_oc(e):true">description</a></code>
</p></td>
            <td><p class="para">
  警告的信息的内容
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW10" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_41&quot;;return this.s_oc?this.s_oc(e):true">text</a></code>
</p></td>
            <td><p class="para">
  简单的描述按钮的动作
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW11" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_42&quot;;return this.s_oc?this.s_oc(e):true">title</a></code>
</p></td>
            <td><p class="para">
            
  标题，简单的描述一个警告的目的
</p></td>
        </tr>
    </tbody>
  </table>

####警告模板的例子：
#####列表2-2 是用TVML表示的alertTemplate的例子，图2-2 对应的显示效果。
列表2-2

 <ol class="code-lines">
            <li><code class="code-voice">&lt;document&gt;</code></li>
            <li><code class="code-voice">   &lt;alertTemplate&gt;</code></li>
            <li><code class="code-voice">      &lt;title&gt;Update Available&lt;/title&gt;</code></li>
            <li><code class="code-voice">      &lt;description&gt;Get the latest tvOS version&lt;/description&gt;</code></li>
            <li><code class="code-voice">      &lt;button&gt;</code></li>
            <li><code class="code-voice">         &lt;text&gt;Update Now&lt;/text&gt;</code></li>
            <li><code class="code-voice">      &lt;/button&gt;</code></li>
            <li><code class="code-voice">      &lt;button&gt;</code></li>
            <li><code class="code-voice">         &lt;text&gt;Cancel&lt;/text&gt;</code></li>
            <li><code class="code-voice">      &lt;/button&gt;</code></li>
            <li><code class="code-voice">   &lt;/alertTemplate&gt;</code></li>
            <li><code class="code-voice">&lt;/document&gt;</code></li>
        </ol>
 
图2-2

<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/alertTemplateSS_2x.png" alt="image: ../Art/alertTemplateSS_2x.png" width="680" height="387">






        
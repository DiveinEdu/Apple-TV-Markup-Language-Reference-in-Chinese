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

####合辑模板
######合辑模板用来显示这样一些信息，一个产品由不同的块组成。例如显示一个专辑以及它里面所有歌曲，它的头部信息显示屏幕的左上方，里面显示了通用的产品信息，在头部下面直接显示几块区域，比如其中一个显示所有的歌。产品相关的内容显示屏幕右边，包括图片和按钮，用户通这些跟产品进行交互。比如播发和购买按钮。如图4-1 显示合辑模板基本的布局。

######图4-1 合辑模板
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/ATV_temps_compilation_2x.png" alt="image: ../Art/ATV_temps_compilation_2x.png" width="678" height="426">

#####合辑模板中主要元素
######列表4-1，用TVML表示一些主要的元素。 表格4-1 对主要元素进行说明。

######列表4-1 
<ol class="code-lines">
            <li><code class="code-voice">&lt;compilationTemplate&gt;</code></li>
            <li><code class="code-voice">   &lt;background&gt;</code></li>
            <li><code class="code-voice">      …</code></li>
            <li><code class="code-voice">   &lt;/background&gt;</code></li>
            <li><code class="code-voice">   &lt;list&gt;</code></li>
            <li><code class="code-voice">      &lt;relatedContent&gt;</code></li>
            <li><code class="code-voice">         &lt;itemBanner&gt;</code></li>
            <li><code class="code-voice">            …</code></li>
            <li><code class="code-voice">         &lt;/itemBanner&gt;</code></li>
            <li><code class="code-voice">      &lt;/relatedContent&gt;</code></li>
            <li><code class="code-voice">      &lt;header&gt;</code></li>
            <li><code class="code-voice">         …</code></li>
            <li><code class="code-voice">      &lt;/header&gt;</code></li>
            <li><code class="code-voice">      &lt;section&gt;</code></li>
            <li><code class="code-voice">         &lt;header&gt;</code></li>
            <li><code class="code-voice">            &lt;title&gt;Title&lt;/title&gt;</code></li>
            <li><code class="code-voice">         &lt;/header&gt;</code></li>
            <li><code class="code-voice">         &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">            …</code></li>
            <li><code class="code-voice">         &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">      &lt;/section&gt;</code></li>
            <li><code class="code-voice">   &lt;/list&gt;</code></li>
            <li><code class="code-voice">&lt;/compilationTemplate&gt;</code></li>
        </ol>
        
######表格4-1，合辑模型元素的描述

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
  <code class="code-voice"><a href="CompoundBackgroundElements.html#//apple_ref/doc/uid/TP40015064-CH24-SW5" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_39&quot;;return this.s_oc?this.s_oc(e):true">background</a></code>
</p></td>
            <td><p class="para">
  背影元素，譬如 <code class="code-voice"><a href="CompoundBackgroundElements.html#//apple_ref/doc/uid/TP40015064-CH24-SW4" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_40&quot;;return this.s_oc?this.s_oc(e):true">audio</a></code>.
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CompoundBannerHeaderElements.html#//apple_ref/doc/uid/TP40015064-CH23-SW11" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_41&quot;;return this.s_oc?this.s_oc(e):true">header</a></code>
</p></td>
            <td><p class="para">
            描述列表里的东西
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CompoundBannerHeaderElements.html#//apple_ref/doc/uid/TP40015064-CH23-SW2" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_42&quot;;return this.s_oc?this.s_oc(e):true">itemBanner</a></code>
</p></td>
            <td><p class="para">
            产品信息各行元素，譬如按钮信息，靠屏幕的右边显示
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW24" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_43&quot;;return this.s_oc?this.s_oc(e):true">list</a></code>
</p></td>
            <td><p class="para">
            它包涵除去background之外合辑元素。
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="LockupElements.html#//apple_ref/doc/uid/TP40015064-CH10-SW5" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_44&quot;;return this.s_oc?this.s_oc(e):true">listItemLockup</a></code>
</p></td>
            <td><p class="para">
            它能包涵一些元素，在列表里创建一项
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CompoundInformationElements.html#//apple_ref/doc/uid/TP40015064-CH22-SW11" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_45&quot;;return this.s_oc?this.s_oc(e):true">relatedContent</a></code>
</p></td>
            <td><p class="para">
  Element containing all elements displayed along the right side of the screen.
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW26" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_46&quot;;return this.s_oc?this.s_oc(e):true">section</a></code>
</p></td>
            <td><p class="para">
            组织其他元素，主要用于布局。
</p></td>
        </tr>
    </tbody>
  </table>

#####合辑模板例子
######列表4-2 用TVML做的一个compilationTemplate例子。这个例子在左边显示了一个专辑信息的列表和一个歌曲列表。右边显示专辑的图片和按钮提示用户去购买，点击rate,或者拖曳音乐。图4-2，是显示效果。

######列表4-2：

<ol class="code-lines">
            <li><code class="code-voice">&lt;document&gt;</code></li>
            <li><code class="code-voice">   &lt;compilationTemplate theme="light"&gt;</code></li>
            <li><code class="code-voice">      &lt;list&gt;</code></li>
            <li><code class="code-voice">         &lt;relatedContent&gt;</code></li>
            <li><code class="code-voice">            &lt;itemBanner&gt;</code></li>
            <li><code class="code-voice">               &lt;heroImg src="path to images on your server/Car_Movie_720x1080" /&gt;</code></li>
            <li><code class="code-voice">               &lt;row&gt;</code></li>
            <li><code class="code-voice">                  &lt;buttonLockup&gt;</code></li>
            <li><code class="code-voice">                     &lt;badge src="resource://button-add"/&gt;</code></li>
            <li><code class="code-voice">                     &lt;title&gt;Add&lt;/title&gt;</code></li>
            <li><code class="code-voice">                  &lt;/buttonLockup&gt;</code></li>
            <li><code class="code-voice">                  &lt;buttonLockup&gt;</code></li>
            <li><code class="code-voice">                     &lt;badge src="resource://button-rate"/&gt;</code></li>
            <li><code class="code-voice">                     &lt;title&gt;Rate&lt;/title&gt;</code></li>
            <li><code class="code-voice">                  &lt;/buttonLockup&gt;</code></li>
            <li><code class="code-voice">                  &lt;buttonLockup&gt;</code></li>
            <li><code class="code-voice">                     &lt;badge src="resource://button-shuffle"/&gt;</code></li>
            <li><code class="code-voice">                     &lt;title&gt;Shuffle&lt;/title&gt;</code></li>
            <li><code class="code-voice">                  &lt;/buttonLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;/row&gt;</code></li>
            <li><code class="code-voice">            &lt;/itemBanner&gt;</code></li>
            <li><code class="code-voice">         &lt;/relatedContent&gt;</code></li>
            <li><code class="code-voice">         &lt;header&gt;</code></li>
            <li><code class="code-voice">            &lt;title&gt;WWDC Roadtrip Soundtrack&lt;/title&gt;</code></li>
            <li><code class="code-voice">            &lt;subtitle&gt;Various Artists&lt;/subtitle&gt;</code></li>
            <li><code class="code-voice">            &lt;row&gt;</code></li>
            <li><code class="code-voice">               &lt;text&gt;Instrumental&lt;/text&gt;</code></li>
            <li><code class="code-voice">               &lt;text&gt;5 Songs&lt;/text&gt;</code></li>
            <li><code class="code-voice">               &lt;text&gt;2015&lt;/text&gt;</code></li>
            <li><code class="code-voice">            &lt;/row&gt;</code></li>
            <li><code class="code-voice">         &lt;/header&gt;</code></li>
            <li><code class="code-voice">         &lt;section&gt;</code></li>
            <li><code class="code-voice">            &lt;description&gt;Songs from your favorite movie&lt;/description&gt;</code></li>
            <li><code class="code-voice">         &lt;/section&gt;</code></li>
            <li><code class="code-voice">         &lt;section&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;ordinal minLength="2"&gt;1&lt;/ordinal&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;Opening sequence&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;11:14&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;ordinal minLength="2"&gt;2&lt;/ordinal&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;Fight song&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;3:47&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;ordinal minLength="2"&gt;3&lt;/ordinal&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;Love theme&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;6:48&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;ordinal minLength="2"&gt;4&lt;/ordinal&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;Car chase&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;5:21&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;ordinal minLength="2"&gt;5&lt;/ordinal&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;End credit theme&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;8:03&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">         &lt;/section&gt;</code></li>
            <li><code class="code-voice">      &lt;/list&gt;</code></li>
            <li><code class="code-voice">   &lt;/compilationTemplate&gt;</code></li>
            <li><code class="code-voice">&lt;/document&gt;</code></li>
        </ol>
        
        
图4-2：

<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/compilationTemplateSS_2x.png" alt="image: ../Art/compilationTemplateSS_2x.png" width="680" height="387">



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

####目录模板（catalogTemplate）

#####用目录模板去显示产品的分类信息。比如一个电影的目录提供了电视剧，喜剧和所有分类，所有分类都显示在它们的块中，并且显示在屏幕的左侧，属于某个选中的分类的图片信息显示在屏幕右侧。图3-1，显示一个基本的catalogTemplate的布局。

图3-1
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/ATV_temps_catalog_2x.png" alt="image: ../Art/ATV_temps_catalog_2x.png" width="678" height="426">

#####catalogTemplate的主要元素
######列表3-1 用TVML格式显示了这些元素，表格3-1是对这些元素的一个描述。

#####列表3-1
<ol class="code-lines">
            <li><code class="code-voice">&lt;catalogTemplate&gt;</code></li>
            <li><code class="code-voice">   &lt;banner&gt;</code></li>
            <li><code class="code-voice">      &lt;title&gt;…&lt;/title&gt;</code></li>
            <li><code class="code-voice">   &lt;/banner&gt;</code></li>
            <li><code class="code-voice">   &lt;list&gt;</code></li>
            <li><code class="code-voice">      &lt;section&gt;</code></li>
            <li><code class="code-voice">         &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">            …</code></li>
            <li><code class="code-voice">         &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">      &lt;/section&gt;</code></li>
            <li><code class="code-voice">      &lt;section&gt;</code></li>
            <li><code class="code-voice">         &lt;header&gt;</code></li>
            <li><code class="code-voice">            &lt;…</code></li>
            <li><code class="code-voice">         &lt;/header&gt;</code></li>
            <li><code class="code-voice">         &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">            …</code></li>
            <li><code class="code-voice">         &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">      &lt;/section&gt;</code></li>
            <li><code class="code-voice">   &lt;/list&gt;</code></li>
            <li><code class="code-voice">&lt;/catalogTemplate&gt;</code></li>
        </ol>
        
######表格3-1

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
  <code class="code-voice"><a href="CompoundBannerHeaderElements.html#//apple_ref/doc/uid/TP40015064-CH23-SW1" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_39&quot;;return this.s_oc?this.s_oc(e):true">banner</a></code>
</p></td>
            <td><p class="para">
            分类的描述信息，比如电影
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CompoundBannerHeaderElements.html#//apple_ref/doc/uid/TP40015064-CH23-SW11" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_40&quot;;return this.s_oc?this.s_oc(e):true">header</a></code>
</p></td>
            <td><p class="para">
  描述页面的一个部分的描述信息。
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW24" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_41&quot;;return this.s_oc?this.s_oc(e):true">list</a></code>
</p></td>
            <td><p class="para">
            这元素包括了除banner以外的信息
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="LockupElements.html#//apple_ref/doc/uid/TP40015064-CH10-SW5" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_42&quot;;return this.s_oc?this.s_oc(e):true">listItemLockup</a></code>
</p></td>
            <td><p class="para">
            这个元素包括了list左边的内容，包括标题，标签，以及内容
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW26" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_43&quot;;return this.s_oc?this.s_oc(e):true">section</a></code>
</p></td>
            <td><p class="para">
            这个元素把相关的一些信息组织成一块，方便布局。
</p></td>
        </tr>
    </tbody>
  </table>
  
####目录模板的例子：

列表3-2，用TVML表示的catalogTemplate例子。 例子的标题在页面顶部，左边有两个选项表式电影的分类。分别是所有和喜剧，被选中的分类的海报用网格显示在页面的右边。图3-2它的一个显示效果。

######列表3-2
<ol class="code-lines">
            <li><code class="code-voice">&lt;document&gt;</code></li>
            <li><code class="code-voice">   &lt;catalogTemplate&gt;</code></li>
            <li><code class="code-voice">      &lt;banner&gt;</code></li>
            <li><code class="code-voice">         &lt;title&gt;Movies&lt;/title&gt;</code></li>
            <li><code class="code-voice">      &lt;/banner&gt;</code></li>
            <li><code class="code-voice">      &lt;list&gt;</code></li>
            <li><code class="code-voice">         &lt;section&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;All Movies&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;6&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">               &lt;relatedContent&gt;</code></li>
            <li><code class="code-voice">                  &lt;grid&gt;</code></li>
            <li><code class="code-voice">                     &lt;section&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_A.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 1&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_B.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 2&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_C.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 3&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 4&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_C.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 5&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 6&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                     &lt;/section&gt;</code></li>
            <li><code class="code-voice">                  &lt;/grid&gt;</code></li>
            <li><code class="code-voice">               &lt;/relatedContent&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">            &lt;listItemLockup&gt;</code></li>
            <li><code class="code-voice">               &lt;title&gt;Comedies&lt;/title&gt;</code></li>
            <li><code class="code-voice">               &lt;decorationLabel&gt;4&lt;/decorationLabel&gt;</code></li>
            <li><code class="code-voice">               &lt;relatedContent&gt;</code></li>
            <li><code class="code-voice">                  &lt;grid&gt;</code></li>
            <li><code class="code-voice">                     &lt;section&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_B.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 2&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_A.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 1&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 4&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                        &lt;lockup&gt;</code></li>
            <li><code class="code-voice">                           &lt;img src="path to images on your server/Car_Movie_250x375_C.png" width="250" height="376" /&gt;</code></li>
            <li><code class="code-voice">                           &lt;title&gt;Movie 3&lt;/title&gt;</code></li>
            <li><code class="code-voice">                        &lt;/lockup&gt;</code></li>
            <li><code class="code-voice">                     &lt;/section&gt;</code></li>
            <li><code class="code-voice">                  &lt;/grid&gt;</code></li>
            <li><code class="code-voice">               &lt;/relatedContent&gt;</code></li>
            <li><code class="code-voice">            &lt;/listItemLockup&gt;</code></li>
            <li><code class="code-voice">         &lt;/section&gt;</code></li>
            <li><code class="code-voice">      &lt;/list&gt;</code></li>
            <li><code class="code-voice">   &lt;/catalogTemplate&gt;</code></li>
            <li><code class="code-voice">&lt;/document&gt;</code></li>
        </ol>
 
 
图3-2

<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/catalogTemplateSS_2x.png" alt="image: ../Art/catalogTemplateSS_2x.png" width="680" height="387">




####descriptiveAlertTemplate
#####descriptiveAlertTemplate 用于描述显示一些重要的信息，比如一些提供服务页面的弹出条款信息。标题显示在屏幕的顶部，在它面直接显示一大段文本区,在屏幕的底陪有一个放按钮的区域。图5-1，显示-个descriptiveAlertTemplate的基本结构。

#####图5-1 descriptiveAlertTemplate
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/ATV_temps_descriptive_2x.png" alt="image: ../Art/ATV_temps_descriptive_2x.png" width="678" height="426">

#####descriptiveAlertTemplate 中主要元素的描述
#####列表5-1 显示TVML标记的主要元素，表5-1 对这些元素的描述

#####列表5-1
<ol class="code-lines">
            <li><code class="code-voice">&lt;descriptiveAlertTemplate&gt;</code></li>
            <li><code class="code-voice">   &lt;title&gt;Title&lt;/title&gt;</code></li>
            <li><code class="code-voice">   &lt;img /&gt;</code></li>
            <li><code class="code-voice">   &lt;description&gt;Description&lt;/description&gt;</code></li>
            <li><code class="code-voice">   &lt;row&gt;</code></li>
            <li><code class="code-voice">      &lt;button&gt;</code></li>
            <li><code class="code-voice">         …</code></li>
            <li><code class="code-voice">      &lt;/button&gt;</code></li>
            <li><code class="code-voice">   &lt;/row&gt;</code></li>
            <li><code class="code-voice">&lt;/descriptiveAlertTemplate&gt;</code></li>
        </ol>
        
#####表5-1

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
            模板上的一个按钮,用户通常用它拒绝警告信息，或者被带另一个新的模板页
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW8" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_40&quot;;return this.s_oc?this.s_oc(e):true">description</a></code>
</p></td>
            <td><p class="para">
  警告的内容
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH19-SW6" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_41&quot;;return this.s_oc?this.s_oc(e):true">img</a></code>
</p></td>
            <td><p class="para">
 	警告相关的图片
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CoumpoundDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH18-SW17" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_42&quot;;return this.s_oc?this.s_oc(e):true">row</a></code>
</p></td>
            <td><p class="para">
  显示按钮的行
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW11" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_43&quot;;return this.s_oc?this.s_oc(e):true">title</a></code>
</p></td>
            <td><p class="para">
  警告页面的标题
</p></td>
        </tr>
    </tbody>
  </table>
  
#####descriptiveAlertTemplate 的例子
#####列表5-2 显示descriptiveAlertTemplate 的TVML例子。图5-2，展示的效果

#####列表5-2

<ol class="code-lines">
            <li><code class="code-voice">&lt;document&gt;</code></li>
            <li><code class="code-voice">   &lt;descriptiveAlertTemplate&gt;</code></li>
            <li><code class="code-voice">      &lt;title&gt;Terms of Service&lt;/title&gt;</code></li>
            <li><code class="code-voice">      &lt;description&gt;Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum&lt;/description&gt;</code></li>
            <li><code class="code-voice">      &lt;row&gt;</code></li>
            <li><code class="code-voice">         &lt;button&gt;</code></li>
            <li><code class="code-voice">            &lt;text&gt;Accept&lt;/text&gt;</code></li>
            <li><code class="code-voice">         &lt;/button&gt;</code></li>
            <li><code class="code-voice">         &lt;button&gt;</code></li>
            <li><code class="code-voice">            &lt;text&gt;Decline&lt;/text&gt;</code></li>
            <li><code class="code-voice">         &lt;/button&gt;</code></li>
            <li><code class="code-voice">      &lt;/row&gt;</code></li>
            <li><code class="code-voice">   &lt;/descriptiveAlertTemplate&gt;</code></li>
            <li><code class="code-voice">&lt;/document&gt;</code></li>
        </ol>
        
#####图5-2
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/descriptiveAlertTemplateSS_2x.png" alt="image: ../Art/descriptiveAlertTemplateSS_2x.png" width="680" height="387">
  
  
  
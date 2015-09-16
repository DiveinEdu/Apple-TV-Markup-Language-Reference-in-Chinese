####formTemplate
#####使用表格模板（formTemplate）去收集用户的信息。例如当你的app只有通过密码才访问时，banner区域包括一引起产品相关的图片和描述。banner下面有一文本框，用户使自动生成的键盘直接输入文本，使用页面下面的按钮来跟用户做交互。图7-1，显示一个forTemplate 页面的基本布局。

#####7-1 forTemplate
<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/ATV_temps_form_2x.png" alt="image: ../Art/ATV_temps_form_2x.png" width="678" height="426">

#####formTemplate中的主要元素
#####列表7-1， 显示用TVML格式标记的主要元素，表7-1，主要元素的描述。

#####列表7-1
<ol class="code-lines">
            <li><code class="code-voice">&lt;formTemplate&gt;</code></li>
            <li><code class="code-voice">   &lt;banner&gt;</code></li>
            <li><code class="code-voice">      &lt;img /&gt;</code></li>
            <li><code class="code-voice">      &lt;description&gt;…&lt;description&gt;</code></li>
            <li><code class="code-voice">   &lt;/banner&gt;</code></li>
            <li><code class="code-voice">   &lt;textField&gt;…&lt;/textField&gt;</code></li>
            <li><code class="code-voice">   &lt;footer&gt;…&lt;/footer&gt;</code></li>
            <li><code class="code-voice">&lt;/formTemplate&gt;</code></li>
        </ol>
        
#####表7-1
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
            这个信息显示在屏幕的顶部，通常地用于给用户做一个介绍。
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleElements.html#//apple_ref/doc/uid/TP40015064-CH4-SW8" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_40&quot;;return this.s_oc?this.s_oc(e):true">description</a></code>
</p></td>
            <td><p class="para">
            描述用户将输入的信息
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="CompoundBannerHeaderElements.html#//apple_ref/doc/uid/TP40015064-CH23-SW4" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_41&quot;;return this.s_oc?this.s_oc(e):true">footer</a></code>
</p></td>
            <td><p class="para">
            信息显示在屏幕的底部，譬如提交按钮，它是用提交用户在文本框中输入的信息。
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleDisplayElements.html#//apple_ref/doc/uid/TP40015064-CH19-SW6" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_42&quot;;return this.s_oc?this.s_oc(e):true">img</a></code>
</p></td>
            <td><p class="para">
  产品的图片
</p></td>
        </tr>
        <tr>
            <td scope="row"><p class="para">
  <code class="code-voice"><a href="SimpleMultimediaElements.html#//apple_ref/doc/uid/TP40015064-CH20-SW6" data-renderer-version="1" onclick="s_objectID=&quot;https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/A_43&quot;;return this.s_oc?this.s_oc(e):true">textField</a></code>
</p></td>
            <td><p class="para">
  用户输入的文本框
</p></td>
        </tr>
    </tbody>
  </table>
  
  
#####formTemplate例子
列表7-2 显示TVML实现的formTemplate例子。用于交互的键盘是自动生成的，屏幕底部的按钮是提交用户输入的。修改你的javascript 文件接受用户的输入，要想了解更多的javascript功能，点击 <a href="https://developer.apple.com/library/prerelease/tvos/documentation/TVMLJS/Reference/TVJSFrameworkReference/index.html#//apple_ref/doc/uid/TP40016076">TVJS Framework </a> 图7-2 显示是输出的效果

#####列表7-2
<ol class="code-lines">
            <li><code class="code-voice">&lt;document&gt;</code></li>
            <li><code class="code-voice">   &lt;formTemplate&gt;</code></li>
            <li><code class="code-voice">      &lt;banner&gt;</code></li>
            <li><code class="code-voice">         &lt;img src="path to images on your server/Car_Movie_800X400.png" width="800" height="400"/&gt;</code></li>
            <li><code class="code-voice">         &lt;description&gt;Enter email for access&lt;/description&gt;</code></li>
            <li><code class="code-voice">      &lt;/banner&gt;</code></li>
            <li><code class="code-voice">      &lt;textField&gt;tclark@example.com&lt;/textField&gt;</code></li>
            <li><code class="code-voice">      &lt;footer&gt;</code></li>
            <li><code class="code-voice">         &lt;button&gt;</code></li>
            <li><code class="code-voice">            &lt;text&gt;Submit&lt;/text&gt;</code></li>
            <li><code class="code-voice">         &lt;/button&gt;</code></li>
            <li><code class="code-voice">      &lt;/footer&gt;</code></li>
            <li><code class="code-voice">   &lt;/formTemplate&gt;</code></li>
            <li><code class="code-voice">&lt;/document&gt;</code></li>
        </ol>

图7-2

<img src="https://developer.apple.com/library/prerelease/tvos/documentation/LanguagesUtilities/Conceptual/ATV_Template_Guide/Art/formTemplateSS_2x.png" alt="image: ../Art/formTemplateSS_2x.png" width="680" height="387">











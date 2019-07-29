# HTML5
## 一个HTML5的例子
```
<!DOCTYPE HTML>
<html>
<body>

<video width="320" height="240" controls="controls">
  <source src="movie.ogg" type="video/ogg">
  <source src="movie.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

</body>
</html>
```


## HTML 5简介

### 什么是 HTML5？
HTML5 将成为 HTML、XHTML 以及 HTML DOM 的新标准。
HTML 的上一个版本诞生于 1999 年。自从那以后，Web 世界已经经历了巨变。
HTML5 仍处于完善之中。然而，大部分现代浏览器已经具备了某些 HTML5 支持。

### HTML5是如何起步的？
HTML5 是 W3C 与 WHATWG 合作的结果。

WHATWG 致力于 web 表单和应用程序，而 W3C 专注于 XHTML 2.0。在 2006 年，双方决定进行合作，来创建一个新版本的 HTML。

为 HTML5 建立的一些规则：

+ 新特性应该基于 HTML、CSS、DOM 以及 JavaScript。
+ 减少对外部插件的需求（比如 Flash）
+ 更优秀的错误处理
+ 更多取代脚本的标记
+ HTML5 应该独立于设备
+ 开发进程应对公众透明

### 新特性
HTML5 中的一些有趣的新特性：
+ 用于绘画的 canvas 元素
+ 用于媒介回放的 video 和 audio 元素
+ 对本地离线存储的更好的支持
+ 新的特殊内容元素，比如 article、footer、header、nav、section
+ 新的表单控件，比如 calendar、date、time、email、url、search



## HTML5新增标签

| **标签**     | **描述**                                           |
| ------------ | -------------------------------------------------- |
| <article>    | 定义article                                        |
| <aside>      | 定义页面内容之外的内容。                           |
| <audio>      | 定义声音内容。                                     |
| <bdi>        | 定义文本的文本方向，使其脱离其周围文本的方向设置。 |
| <canvas>     | 定义图形。                                         |
| <command>    | 定义命令按钮。                                     |
| <datalist>   | 定义下拉列表。                                     |
| <details>    | 定义元素的细节。                                   |
| <embed>      | 定义外部交互内容或插件。                           |
| <figcaption> | 定义   figure 元素的标题。                         |
| <figure>     | 定义媒介内容的分组，以及它们的标题。               |
| <footer>     | 定义   section 或 page 的页脚。                    |
| <header>     | 定义   section 或 page 的页眉。                    |
| <hgroup>     | 定义有关文档中的   section 的信息。                |
| <keygen>     | 定义生成密钥。                                     |
| <main>      | 定义文档的主要内容。                         |
| <mark>       | 定义有记号的文本。                                 |
| <meter>      | 定义预定义范围内的度量。                           |
| <nav>        | 定义导航链接。                                     |
| <output>     | 定义输出的一些类型。                               |
| <progress>   | 定义任何类型的任务的进度。                         |
| <rp>         | 定义若浏览器不支持 ruby 元素显示的内容。           |
| <rt>         | 定义 ruby 注释的解释。                             |
| <ruby>       | 定义 ruby 注释。                                   |
| <section>    | 定义   section。                                   |
| <source>     | 定义媒介源。                                       |
| <summary>    | 定义   details 元素的标题。                        |
| <time>       | 定义日期/时间。                                    |
| <track>      | 定义用在媒体播放器中的文本轨道。                   |
| <video>      | 定义视频。                                         |

### article

**1、定义和用法：**

<article> article元素代表文档、页面或应用程序中独立的、完整的、可以独自被外部引用的内容。

可能的 article 实例：

- 论坛帖子
- 报纸文章
- 博客条目
- 用户评论

**2、实例**

```
<article>
      <header>
            <h1>article元素使用方法</h1>
            <p>发表日期：<time pubdate="pubdate">2019/05/20</time></p>
      </header>
      <p>article元素是什么？怎样使用article元素？……</p>
      <section>
            <h2>评论</h2>
            <article>
                  <header>
                        <h3>发表者：Felixlu</h3>
                        <p><time pubdate datetime="2019-05-20T:21-26:00">1小时前</time></p>
                  </header>
                  <p>这篇文章很不错啊，顶一下！</p>
            </article>
            <article>
                  <header>
                        <h3>发表者：神秘唯一</h3>
                        <p><time pubdate datetime="2019-05-20T:21-26:00">1小时前</time></p>
                  </header>
                  <p>这篇文章很不错啊，对article解释的很详细</p>
            </article>
      </section>
</article>
```
### section

**1、定义和用法：**

section元素用于对网站或应用程序中页面上的内容进行分块。一个section元素通常由内容及其标题组成。但section元素并非一个普通的容器元素；当一个内容需要被直接定义样式或通过脚本定义行为时，推荐使用div而非section元素。section元素中的内容可以单独存储到数据库中或输出到word文档中。

**2、实例**

通常不推荐为那些没有标题的内容使用section元素。
section元素的作用是对页面上的内容进行分块，或者说对文章进行分段，请不要与有着自己的完整的、独立的内容的article元素混淆。

```
<section>
      <h1>section元素使用方法</h1>
      <p>什么时候用section元素？怎样合理使用section元素?</p>
</section>

<article>
      <h1>article元素与section元素的使用方法</h1>
      <p>何时使用article元素？何时使用section元素…..</p>
      <section>
            <h2>article元素使用方法</h2>
            <p>article元素代表文档、页面或应用程序中独立的、完整的、可以独自被外部引用的内容。</p>
      </section>
      <section>
            <h2>section元素使用方法</h2>
            <p> section元素用于对网站或应用程序中页面上的内容进行分块。</p>
      </section>
</article>
```
**3、section 使用禁忌**

+ 不要将section元素用作设置样式的页面容器，那是div元素的工作。
+ 如果article元素、aside元素或nav元素更符合使用条件，不要使用section元素。
+ 不要为没有标题的内容区块使用section元素。

**4、section 与 article 的区别**

在HTML5中，article元素可以看成是一种特殊类型的section元素，它比 section元素更强调独立性。即section元素强调分段或分块，而article强调独立性。具体来说，如果一块内容相对来说比较独立的、完整的时候，应该使用article元素，但是如果你想将一块内容分成几段的时候，应该使用section元素。另外，在HTML5中，div元素变成了一种容器，当使用CSS样式的时候，可以对这个容器进行一个总体的CSS样式的套用。

### aside

**1、定义和用法**

HTML<aside>元素表示一个页面的一部分， 它的内容跟这个页面的其它内容的关联性不强，或者是没有关联，单独存在。<aside>元素通常显示成侧边栏(sidebar)或一些插入补充内容。通常用来在侧边栏显示一些定义，比如目录、索引、术语表等；也可以用来显示相关的广告宣传，作者的介绍，Web应用，相关链接，当前页内容简介等。

不要使用<aside>元素标记括号中的文字，因为这种类型的文本被认为是主内容的一部分。

**2、实例**
```
<article>  
  <p>  
    The Disney movie <em>The Little Mermaid</em> was   
    first released to theatres in 1989.   
  </p>  
  <aside>  
    The movie earned $87 million during its initial release.   
  </aside>  
  <p>  
    More info about the movie...   
  </p>  
</article>
```
### main

**1、定义和用法**

<main> 标签规定文档的主要内容。

<main> 元素中的内容对于文档来说应当是唯一的。它不应包含在文档中重复出现的内容，比如侧栏、导航栏、版权信息、站点标志或搜索表单。
**注释：**在一个文档中，不能出现一个以上的 <main> 元素。<main> 元素不能是以下元素的后代：<article>、<aside>、<footer>、<header> 或 <nav>。

**2、实例**

```
<main>
  <h1>Web Browsers</h1>
  <p>Google Chrome、Firefox 以及 Internet Explorer 是目前最流行的浏览器。</p>

  <article>
    <h1>Google Chrome</h1>
    <p>Google Chrome 是由 Google 开发的一款免费的开源 web 浏览器，于 2008 年发布。</p>
  </article>

  <article>
    <h1>Internet Explorer</h1>
    <p>Internet Explorer 由微软开发的一款免费的 web 浏览器，发布于 1995 年。</p>
  </article>

  <article>
    <h1>Mozilla Firefox</h1>
    <p>Firefox 是一款来自 Mozilla 的免费开源 web 浏览器，发布于 2004 年。</p>
  </article>
</main> 
```

### header

**1、定义和用法**

标签 <header> 定义文档的页眉（介绍信息）。

**2、实例**

```
<header>
  <h1>Welcome to my homepage</h1>
  <p>My name is Donald Duck</p>
</header>
<p>The rest of my home page...</p>
```
### footer

**1、定义和用法**

标签 <footer> 定义文档或节的页脚。

元素 <footer> 应当含有其包含元素的信息。

页脚通常包含文档的作者、版权信息、使用条款链接、联系信息等等。

您可以在一个文档中使用多个 <footer> 元素。

**2、实例**

```
<footer>
  <p>Posted by: GP-1011</p>
  <p>Contact information: <a href="mailto:someone@example.com">someone@example.com</a>.</p>
</footer>
```

### nav

**1、定义和用法**

`<nav>`是与导航相关的，所以一般用于网站导航布局。同时完全就像使用`div`标签、`span`标签一样来使用`<nav>`标签，可添加`id`或`class`。而与`div`标签又有不同处是，此标签一般只用于导航相关地方使用，所以在一个html网页布局中可能就使用在导航条处，或与导航条相关的地方布局使用。

**2、实例**
```
<nav> 
  <ul> 
    <li>首页</li> 
    <li>栏目名称</li> 
    <li>联系我们</li> 
  </ul> 
</nav> 
```

### datalist

**1、定义和用法**

<datalist> 标签定义选项列表。与 input 元素配合使用该元素，来定义 input 可能的值。

datalist 及其选项不会被显示出来，它仅仅是合法的输入值列表。

使用 input 元素的 list 属性来绑定 datalist。

**2、实例**
```
<input id="myCar" list="cars" />

<datalist id="cars">
  <option value="BMW">
  <option value="Ford">
  <option value="Volvo">
</datalist>
```

### command

**1、定义和用法**

在HTML5中，<command>标签是用来表示用户能够调用的命令，可以定义命令按钮，比如单选按钮、复选框或按钮。<command>标签在<menu>元标签中才是可见的，它还可以规定键盘快捷键。<command> 标签是html 5中新增标签，目前只有在IE 9中支持。

**2、实例**
```
<menu>
  <command type="command" label="Save" onclick="save()">Save</command>
</menu>
```

### details & summary

**1、定义和用法**

`<details>` 标签 用于描述文档或文档某个部分的细节，与 <summary> 标签 配合使用可以为 details 定义标题。标题是可见的，用户点击标题时，会显示出 details。
`<details>` 标签 拥有 open 属性，"details" 元素默认是隐藏的，设置 open 属性后，可以定义"details" 元素默认可见，与checkbox定义checked属性是一个道理。

**2、实例**
```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <title>Title</title>
    <style>
        ::-webkit-details-marker{
            display:none;
        }
        ::-moz-list-bullet {
            font-size: 0;
            float: left;
        }
        summary{
            font-weight:bolder;
            cursor:pointer;
            user-select: none;
            outline: 0;
        }
        li{
            list-style: none;
        }
    </style>
</head>
<body>
    <details>
        <summary>商品管理</summary>
        <li>商品列表</li>
        <li>添加商品</li>
    </details>
    <details>
        <summary>品牌管理</summary>
        <li>品牌列表</li>
        <li>添加品牌</li>
    </details>
    <details>
        <summary>分类管理</summary>
        <li>分类列表</li>
        <li>添加分类</li>
    </details>
</body>
</html>
```
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>details & summary</title>
  <style>
    div {
        width: 7%;
        margin: 0 auto;
        text-align: center;
    }
    ::-webkit-details-marker {
        display:none;
    }
    ::-moz-list-bullet {
        font-size: 0;
        float: left;
    }
    details {
        position:relative;
        background:#f5f5f5;
    }
    summary {
        font-weight:bolder;
        cursor:pointer;
        user-select: none;
        outline: 0;
    }
    li {
        border:1px solid #eee;
        border-top : 0;
        list-style: none;
    }
    /* 实现动画的原理 */
    summary::after {
        content: '';
        width: 0;
        height: 0;
        line-height: 0;
        font-size: 0;
        border-left: 5px dashed transparent;
        border-right: 5px dashed transparent;
        border-top: 5px solid #000;
        position: absolute;
        top: 44%;
        right: 8%;
        transition:.3s ease-out;
    }
    [open] summary::after {
        transform:rotate(180deg)
    }
    ul {
        max-height: 0;
        padding:0;
        margin-top:0;
        transition: .3s ease-out;
        overflow: hidden;
    }
    [open] + ul {
        max-height: 60px;
    }
  </style>
</head>
<body>
    <div>
        <details open>
            <summary>商品管理</summary>
        </details>
        <ul>
            <li>商品列表</li>
            <li>添加商品</li>
        </ul>
    </div>
    <div>
        <details open>
            <summary>品牌管理</summary>
        </details>
        <ul>
            <li>品牌列表</li>
            <li>添加品牌</li>
        </ul>
    </div>
    <div>
        <details open>
            <summary>分类管理</summary>
        </details>
        <ul>
            <li>分类列表</li>
            <li>添加分类</li>
        </ul>
    </div>
</body>
</html>
```

### hgroup

**1、定义和用法**

hgroup元素是将标题和他的子标题进行分组的元素。hgroup元素一般会把h1-h6的元素进行分组，比如在一个内容区块的标题和他的子标题算是一组。通常情况下，文章只有一个主标题时，是不需要hgroup元素的。

**2、实例**
```
<article>
  <header>
    <hgroup>
      <h1>文章主标题</h1>
      <h2>文章子标题</h2>
    </hgroup>
    <p><time datetime=”2019-05-20”>2019年05月20日</time></p>
  </header>
  <p>文章正文</p>
</article>
```

### figure & figcaption

**1、定义和用法**

`<figure>`  标签规定独立的流内容（图像、图表、照片、代码等等）。

figure 元素的内容应该与主内容相关，但如果被删除，则不应对文档流产生影响。

**2、实例**

hover 例子：https://tympanus.net/Development/HoverEffectIdeas/index2.html
```
<div class="hover-area area-Julia">
  <img src="imgs/21.jpg" height="360" width="480">
  <h3>PASSIONATE<strong>JULIA</strong></h3>
  <ul>
    <li>Julia dances in the deep dark.</li>
    <li>She loves the smell of the ocean</li>
    <li>And dives into the morning light</li>
  </ul>
</div>
```
VS
```
<figure class="effect-julia">
  <img src="img/21.jpg" alt="img21"/>
  <figcaption>
    <h2>Passionate <span>Julia</span></h2>
    <div>
      <p>Julia dances in the deep dark</p>
      <p>She loves the smell of the ocean</p>
      <p>And dives into the morning light</p>
    </div>
    <a href="#">View more</a>
  </figcaption>			
</figure>
```

### mark

**1、定义和用法**

<mark> 标签定义带有记号的文本。请在需要突出显示文本时使用 <m> 标签。

**2、实例**
```
<p>Do not forget to buy <mark>milk</mark> today.</p>
```

### time

**1、定义和用法**

<time> 标签定义公历的时间（24 小时制）或日期，时间和时区偏移是可选的。

该元素能够以机器可读的方式对日期和时间进行编码，这样，举例说，用户代理能够把生日提醒或排定的事件添加到用户日程表中，搜索引擎也能够生成更智能的搜索结果。

**2、实例**

```
<p>我们在每天早上 <time>9:00</time> 开始营业。</p>
<p>我在 <time datetime="2019-02-14">情人节</time> 有个约会。</p>
```

### output

**1、定义和用法**

<output> 标签定义不同类型的输出，比如脚本的输出。

**2、实例**

```
<form oninput="x.value=parseInt(a.value)+parseInt(b.value)">0
   <input type="range" id="a" value="50">100
   +<input type="number" id="b" value="50">
   =<output name="x" for="a b"></output>
</form> 
```

### progress

**1、定义和用法**

<progress> 标签标示任务的进度（进程）。

**2、实例**

```
<progress value="22" max="100"></progress>

样式：
progress {
   color:orange; /*兼容IE10的已完成进度背景*/
   border:none;
   background: #d7d7d7;/*这个属性也可当作Chrome的已完成进度背景，只不过被下面的::progress-bar覆盖了*/      
}

progress::-webkit-progress-bar {
   background: #d7d7d7;
}

progress::-webkit-progress-value,
progress::-moz-progress-bar
{
  background: orange;
}
```

### meter

**1、定义和用法**

<meter> 标签定义已知范围或分数值内的标量测量。也被称为 gauge（尺度）。

例子：磁盘用量、查询结果的相关性，等等。

**注释：**<meter> 标签不应用于指示进度（在进度条中）。如果标记进度条，请使用 <progress> 标签。

**2、实例**
```
<meter value="3" min="0" max="10">十分之三</meter>
<meter value="0.6">60%</meter> 
```

### keygen

**1、定义和用法**

<keygen> 标签规定用于表单的密钥对生成器字段。

当提交表单时，私钥存储在本地，公钥发送到服务器。

**2、实例**
```
<form action="demo_keygen.do" method="get">
  Username: <input type="text" name="usr_name" />
  Encryption: <keygen name="security" />
  <input type="submit" />
</form>
```

### embed

**1、定义和用法**

embed可以用来插入各种多媒体，格式可以是 Midi、Wav、AIFF、AU、MP3等等，Netscape及新版的IE都支持。url为音频或视频文件及其路径，可以是相对路径或绝对路径。

**2、实例**
```
<embed src="your.mid">
```

### source

**1、定义和用法**

<source> 标签为媒介元素（比如 <video> 和 <audio>）定义媒介资源。
<source> 标签允许您规定可替换的视频/音频文件供浏览器根据它对媒体类型或者编解码器的支持进行选择。

**2、实例**
```
<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Your browser does not support the audio element.
 </audio> 
```
### track

**1、定义和用法**

<track> 标签为诸如 video 元素之类的媒介规定外部文本轨道。

用于规定字幕文件或其他包含文本的文件，当媒介播放时，这些文件是可见的。

目前所有主流浏览器都`不支持` <track> 标签。

**2、实例**
```
<video width="320" height="240" controls="controls">
  <source src="forrest_gump.mp4" type="video/mp4" />
  <source src="forrest_gump.ogg" type="video/ogg" />
  <track kind="subtitles" src="subs_chi.srt" srclang="zh" label="Chinese">
  <track kind="subtitles" src="subs_eng.srt" srclang="en" label="English">
</video>
```

### bdi

**1、定义和用法**

bdi 指的是 bidi 隔离。

<bdi> 标签允许您设置一段文本，使其脱离其父元素的文本方向设置。

在发布用户评论或其他您无法完全控制的内容时，该标签很有用。

浏览器支持差。

**2、实例**
```
<ul>
  <li>Username <bdi>Bill</bdi>:80 points</li>
  <li>Username <bdi>Steve</bdi>: 78 points</li>
</ul>
```

### ruby & rp & rb & rt

**1、定义和用法**

<ruby> 标签定义 ruby 注释（中文注音或字符）。

在东亚使用，显示的是东亚字符的发音。

与 <ruby> 以及 <rt> 标签一同使用：

ruby 元素由一个或多个字符（需要一个解释/发音）和一个提供该信息的 rt 元素组成，还包括可选的 rp 元素，定义当浏览器不支持 "ruby" 元素时显示的内容。

<rb> 要注音的对象。

**2、实例**
```
<ruby>
  <rb>千锋教育</rb>
  <rp>(</rp>
  <rt>qian feng jiao yu</rt>
  <rp>)</rp>
</ruby>
```

### video

**1、定义和用法**

`<video>` 标签定义视频，比如电影片段或其他视频流。

**2、实例**
```
<video src="movie.ogg" controls="controls">
您的浏览器不支持 video 标签。
</video>
```

### audio

**1、定义和用法**

`<audio>` 标签定义声音，比如音乐或其他音频流。

**2、实例**

```
<audio src="someaudio.wav">
您的浏览器不支持 audio 标签。
</audio>
```

### canvas

**1、定义和用法**

`<canvas>` 标签定义图形，比如图表和其他图像。
`<canvas>` 标签只是图形容器，您必须使用脚本来绘制图形。

**2、实例**

```
<canvas id="myCanvas"></canvas>

<script type="text/javascript">

var canvas=document.getElementById('myCanvas');
var ctx=canvas.getContext('2d');
ctx.fillStyle='#FF0000';
ctx.fillRect(0,0,80,100);

</script>
```



## HTML5 表单

### HTML5 新的 Input 类型

HTML5 拥有多个新的表单输入类型。这些新特性提供了更好的输入控制和验证：

- email
- url
- number
- range
- Date pickers (date, month, week, time, datetime, datetime-local)
- search
- color

**Input 类型 - email**

email 类型用于应该包含 e-mail 地址的输入域。

在提交表单时，会自动验证 email 域的值。

```
E-mail: <input type="email" name="user_email" />
```

**Input 类型 - url**

url 类型用于应该包含 URL 地址的输入域。

在提交表单时，会自动验证 url 域的值。

```
Homepage: <input type="url" name="user_url" />
```

**Input 类型 - number**

number 类型用于应该包含数值的输入域。

您还能够设定对所接受的数字的限定：

```
Points: <input type="number" name="points" min="1" max="10" />
```

请使用下面的属性来规定对数字类型的限定：

| 属性  | 值       | 描述                                                         |
| :---- | :------- | :----------------------------------------------------------- |
| max   | *number* | 规定允许的最大值                                             |
| min   | *number* | 规定允许的最小值                                             |
| step  | *number* | 规定合法的数字间隔（如果 step="3"，则合法的数是 -3,0,3,6 等） |
| value | *number* | 规定默认值                                                   |

**Input 类型 - range**

range 类型用于应该包含一定范围内数字值的输入域。

range 类型显示为滑动条。

您还能够设定对所接受的数字的限定：

```
<input type="range" name="points" min="1" max="10" />
```

请使用下面的属性来规定对数字类型的限定：

| 属性  | 值       | 描述                                                         |
| :---- | :------- | :----------------------------------------------------------- |
| max   | *number* | 规定允许的最大值                                             |
| min   | *number* | 规定允许的最小值                                             |
| step  | *number* | 规定合法的数字间隔（如果 step="3"，则合法的数是 -3,0,3,6 等） |
| value | *number* | 规定默认值                                                   |

**Input 类型 - Date Pickers（日期选择器）**

HTML5 拥有多个可供选取日期和时间的新输入类型：

- date - 选取日、月、年
- month - 选取月、年
- week - 选取周和年
- time - 选取时间（小时和分钟）
- datetime - 选取时间、日、月、年（UTC 时间）
- datetime-local - 选取时间、日、月、年（本地时间）

下面的例子允许您从日历中选取一个日期：

```
Date: <input type="date" name="user_date" />
```

**Input 类型 - search**

search 类型用于搜索域，比如站点搜索或 Google 搜索。

search 域显示为常规的文本域。

### HTML5 新的表单元素

HTML5 拥有若干涉及表单的元素和属性。

- datalist
- keygen
- output

**datalist 元素**

datalist 元素规定输入域的选项列表。

列表是通过 datalist 内的 option 元素创建的。

如需把 datalist 绑定到输入域，请用输入域的 list 属性引用 datalist 的 id：

```
Webpage: <input type="url" list="url_list" name="link" />
<datalist id="url_list">
<option label="baidu" value="http://www.baidu.com" />
<option label="tencent" value="http://www.qq.com" />
<option label="alibaba" value="http://www.alibaba.com" />
</datalist>
```

**keygen 元素**

keygen 元素的作用是提供一种验证用户的可靠方法。

keygen 元素是密钥对生成器（key-pair generator）。当提交表单时，会生成两个键，一个是私钥，一个公钥。

私钥（private key）存储于客户端，公钥（public key）则被发送到服务器。公钥可用于之后验证用户的客户端证书（client certificate）。

目前，浏览器对此元素的糟糕的支持度不足以使其成为一种有用的安全标准。

```
<form action="demo_form.php" method="get">
Username: <input type="text" name="usr_name" />
Encryption: <keygen name="security" />
<input type="submit" />
</form>
```

**output 元素**

output 元素用于不同类型的输出，比如计算或脚本输出：

```
<output id="result" onforminput="resCalc()"></output>
```

### HTML5 新的表单属性

**新的 form 属性：**

- autocomplete
- novalidate

**新的 input 属性：**

- autocomplete
- autofocus
- form
- form overrides (formaction, formenctype, formmethod, formnovalidate, formtarget)
- height 和 width
- list
- min, max 和 step
- multiple
- pattern (regexp)
- placeholder
- required

**autocomplete 属性**

autocomplete 属性规定 form 或 input 域应该拥有自动完成功能。

**注释：**autocomplete 适用于 <form> 标签，以及以下类型的 <input> 标签：text, search, url, telephone, email, password, datepickers, range 以及 color。

当用户在自动完成域中开始输入时，浏览器应该在该域中显示填写的选项：

```
<form action="demo_form.php" method="get" autocomplete="on">
First name: <input type="text" name="fname" /><br />
Last name: <input type="text" name="lname" /><br />
E-mail: <input type="email" name="email" autocomplete="off" /><br />
<input type="submit" />
</form>
```

**注释：**在某些浏览器中，您可能需要启用自动完成功能，以使该属性生效。

**autofocus 属性**

autofocus 属性规定在页面加载时，域自动地获得焦点。

**注释：**autofocus 属性适用于所有 <input> 标签的类型。

```
User name: <input type="text" name="user_name"  autofocus="autofocus" />
```

**form 属性**

form 属性规定输入域所属的一个或多个表单。

**注释：**form 属性适用于所有 <input> 标签的类型。

form 属性必须引用所属表单的 id：

```
<form action="demo_form.php" method="get" id="user_form">
First name:<input type="text" name="fname" />
<input type="submit" />
</form>
Last name: <input type="text" name="lname" form="user_form" />
```

**注释：**如需引用一个以上的表单，请使用空格分隔的列表。

**表单重写属性**

表单重写属性（form override attributes）允许您重写 form 元素的某些属性设定。

表单重写属性有：

- formaction - 重写表单的 action 属性
- formenctype - 重写表单的 enctype 属性
- formmethod - 重写表单的 method 属性
- formnovalidate - 重写表单的 novalidate 属性
- formtarget - 重写表单的 target 属性

**注释：**表单重写属性适用于以下类型的 <input> 标签：submit 和 image。

```
<form action="demo_form.php" method="get" id="user_form">
E-mail: <input type="email" name="userid" /><br />
<input type="submit" value="Submit" />
<br />
<input type="submit" formaction="demo_admin.php" value="Submit as admin" />
<br />
<input type="submit" formnovalidate="true" value="Submit without validation" />
<br />
</form>
```

**注释：**这些属性对于创建不同的提交按钮很有帮助。

**height 和 width 属性**

height 和 width 属性规定用于 image 类型的 input 标签的图像高度和宽度。

**注释：**height 和 width 属性只适用于 image 类型的 <input> 标签。

```
<input type="image" src="img_submit.gif" width="99" height="99" />
```

**list 属性**

list 属性规定输入域的 datalist。datalist 是输入域的选项列表。

**注释：**list 属性适用于以下类型的 <input> 标签：text, search, url, telephone, email, date pickers, number, range 以及 color。

```
Webpage: <input type="url" list="url_list" name="link" />
<datalist id="url_list">
<option label="baidu" value="http://www.baidu.com" />
<option label="tencent" value="http://www.qq.com" />
<option label="alibaba" value="http://www.alibaba.com" />
</datalist>
```

**min、max 和 step 属性**

min、max 和 step 属性用于为包含数字或日期的 input 类型规定限定（约束）。

max 属性规定输入域所允许的最大值。

min 属性规定输入域所允许的最小值。

step 属性为输入域规定合法的数字间隔（如果 step="3"，则合法的数是 -3,0,3,6 等）。

**注释：**min、max 和 step 属性适用于以下类型的 <input> 标签：date pickers、number 以及 range。

下面的例子显示一个数字域，该域接受介于 0 到 10 之间的值，且步进为 3（即合法的值为 0、3、6 和 9）：

```
Points: <input type="number" name="points" min="0" max="10" step="3" />
```

**multiple 属性**

multiple 属性规定输入域中可选择多个值。

**注释：**multiple 属性适用于以下类型的 <input> 标签：email 和 file。

```
Select images: <input type="file" name="img" multiple="multiple" />
```

**novalidate 属性**

novalidate 属性规定在提交表单时不应该验证 form 或 input 域。

**注释：**novalidate 属性适用于 <form> 以及以下类型的 <input> 标签：text, search, url, telephone, email, password, date pickers, range 以及 color.

```
<form action="demo_form.php" method="get" novalidate="true">
E-mail: <input type="email" name="user_email" />
<input type="submit" />
</form>
```
**pattern 属性**

pattern 属性规定用于验证 input 域的模式（pattern）。

模式（pattern） 是正则表达式。

**注释：**pattern 属性适用于以下类型的 <input> 标签：text, search, url, telephone, email 以及 password。

下面的例子显示了一个只能包含三个字母的文本域（不含数字及特殊字符）：

```
Country code: <input type="text" name="country_code"
pattern="[A-z]{3}" title="Three letter country code" />
```

**placeholder 属性**

placeholder 属性提供一种提示（hint），描述输入域所期待的值。

**注释：**placeholder 属性适用于以下类型的 <input> 标签：text, search, url, telephone, email 以及 password。

提示（hint）会在输入域为空时显示出现，会在输入域获得焦点时消失：

```
<input type="search" name="user_search"  placeholder="Search" />
```
**required 属性**

required 属性规定必须在提交之前填写输入域（不能为空）。

**注释：**required 属性适用于以下类型的 <input> 标签：text, search, url, telephone, email, password, date pickers, number, checkbox, radio 以及 file。

```
Name: <input type="text" name="usr_name" required="required" />
```



## HTML5 全局属性

HTML5 中添加的属性。

| 属性            | 描述                                                   |
| :-------------- | :----------------------------------------------------- |
| contenteditable | 规定元素内容是否可编辑。                               |
| contextmenu     | 规定元素的上下文菜单。上下文菜单在用户点击元素时显示。 |
| data-*          | 用于存储页面或应用程序的私有定制数据。                 |
| draggable       | 规定元素是否可拖动。                                   |
| dropzone        | 规定在拖动被拖动数据时是否进行复制、移动或链接。       |
| hidden          | 隐藏元素                                               |
| spellcheck      | 规定是否对元素进行拼写和语法检查。                     |
| translate       | 规定是否应该翻译元素内容。                             |



## HTML5事件

### window 事件属性

针对 window 对象触发的事件（应用到 <body> 标签）：

| 属性           | 值     | 描述                                  |
| :------------- | :----- | :------------------------------------ |
| onafterprint   | script | 文档打印之后运行的脚本。              |
| onbeforeprint  | script | 文档打印之前运行的脚本。              |
| onbeforeunload | script | 文档卸载之前运行的脚本。              |
| onerror        | script | 在错误发生时运行的脚本。              |
| onhashchange   | script | 当文档已改变时运行的脚本。            |
| onmessage      | script | 在消息被触发时运行的脚本。            |
| onoffline      | script | 当文档离线时运行的脚本。              |
| ononline       | script | 当文档上线时运行的脚本。              |
| onpagehide     | script | 当窗口隐藏时运行的脚本。              |
| onpageshow     | script | 当窗口成为可见时运行的脚本。          |
| onpopstate     | script | 当窗口历史记录改变时运行的脚本。      |
| onredo         | script | 当文档执行撤销（redo）时运行的脚本。  |
| onstorage      | script | 在 Web Storage 区域更新后运行的脚本。 |
| onundo         | script | 在文档执行 undo 时运行的脚本。        |

### Form 事件

由 HTML 表单内的动作触发的事件（应用到几乎所有 HTML 元素，但最常用在 form 元素中）：

| 属性                                                         | 值     | 描述                                             |
| :----------------------------------------------------------- | :----- | :----------------------------------------------- |
| oncontextmenu                                                | script | 当上下文菜单被触发时运行的脚本。                 |
| onformchange                                                 | script | 在表单改变时运行的脚本。                         |
| onforminput                                                  | script | 当表单获得用户输入时运行的脚本。                 |
| oninvalid                                                    | script | 当元素无效时运行的脚本。                         |

### Mouse 事件

由鼠标或类似用户动作触发的事件：

| 属性                                                         | 值     | 描述                                           |
| :----------------------------------------------------------- | :----- | :--------------------------------------------- |
| ondrag                                                       | script | 元素被拖动时运行的脚本。                       |
| ondragend                                                    | script | 在拖动操作末端运行的脚本。                     |
| ondragenter                                                  | script | 当元素元素已被拖动到有效拖放区域时运行的脚本。 |
| ondragleave                                                  | script | 当元素离开有效拖放目标时运行的脚本。           |
| ondragover                                                   | script | 当元素在有效拖放目标上正在被拖动时运行的脚本。 |
| ondragstart                                                  | script | 在拖动操作开端运行的脚本。                     |
| ondrop                                                       | script | 当被拖元素正在被拖放时运行的脚本。             |
| onmousewheel                                                 | script | 当鼠标滚轮正在被滚动时运行的脚本。             |
| onscroll                                                     | script | 当元素滚动条被滚动时运行的脚本。               |

### Media 事件

由媒介（比如视频、图像和音频）触发的事件（适用于所有 HTML 元素，但常见于媒介元素中，比如 <audio>、<embed>、<img>、<object> 以及 <video>）:

| 属性               | 值     | 描述                                                         |
| :----------------- | :----- | :----------------------------------------------------------- |
| oncanplay          | script | 当文件就绪可以开始播放时运行的脚本（缓冲已足够开始时）。     |
| oncanplaythrough   | script | 当媒介能够无需因缓冲而停止即可播放至结尾时运行的脚本。       |
| ondurationchange   | script | 当媒介长度改变时运行的脚本。                                 |
| onemptied          | script | 当发生故障并且文件突然不可用时运行的脚本（比如连接意外断开时）。 |
| onended            | script | 当媒介已到达结尾时运行的脚本（可发送类似“感谢观看”之类的消息）。 |
| onerror            | script | 当在文件加载期间发生错误时运行的脚本。                       |
| onloadeddata       | script | 当媒介数据已加载时运行的脚本。                               |
| onloadedmetadata   | script | 当元数据（比如分辨率和时长）被加载时运行的脚本。             |
| onloadstart        | script | 在文件开始加载且未实际加载任何数据前运行的脚本。             |
| onpause            | script | 当媒介被用户或程序暂停时运行的脚本。                         |
| onplay             | script | 当媒介已就绪可以开始播放时运行的脚本。                       |
| onplaying          | script | 当媒介已开始播放时运行的脚本。                               |
| onprogress         | script | 当浏览器正在获取媒介数据时运行的脚本。                       |
| onratechange       | script | 每当回放速率改变时运行的脚本（比如当用户切换到慢动作或快进模式）。 |
| onreadystatechange | script | 每当就绪状态改变时运行的脚本（就绪状态监测媒介数据的状态）。 |
| onseeked           | script | 当 seeking 属性设置为 false（指示定位已结束）时运行的脚本。  |
| onseeking          | script | 当 seeking 属性设置为 true（指示定位是活动的）时运行的脚本。 |
| onstalled          | script | 在浏览器不论何种原因未能取回媒介数据时运行的脚本。           |
| onsuspend          | script | 在媒介数据完全加载之前不论何种原因终止取回媒介数据时运行的脚本。 |
| ontimeupdate       | script | 当播放位置改变时（比如当用户快进到媒介中一个不同的位置时）运行的脚本。 |
| onvolumechange     | script | 每当音量改变时（包括将音量设置为静音）时运行的脚本。         |
| onwaiting          | script | 当媒介已停止播放但打算继续播放时（比如当媒介暂停已缓冲更多数据）运行脚本 |



## embed

### 一、基本语法
```
embed src = url
```
说明：embed可以用来插入各种多媒体，格式可以是 Midi、Wav、AIFF、AU、MP3等等，Netscape及新版的IE 都支持。url为音频或视频文件及其路径，可以是相对路径或绝对路径。
```
<embed src="your.mid">
```
### 二、属性设置
#### 1、自动播放
语法：autostart=true、false
说明：该属性规定音频或视频文件是否在下载完之后就自动播放。
true：音乐文件在下载完之后自动播放；
false：音乐文件在下载完之后不自动播放。

示例：
```
<embed src="your.mid" autostart=true>
<embed src="your.mid" autostart=false>
```
#### 2、循环播放
语法：loop=正整数、true、false
说明：该属性规定音频或视频文件是否循环及循环次数。
属性值为正整数值时，音频或视频文件的循环次数与正整数值相同；
属性值为true时，音频或视频文件循环；
属性值为false时，音频或视频文件不循环。

示例：
```
<embed src="your.mid" autostart=true loop=2>
<embed src="your.mid" autostart=true loop=true>
<embed src="your.mid" autostart=true loop=false>
```
#### 3、面板显示
语法：hidden=ture、no
说明：该属性规定控制面板是否显示，默认值为no。
ture：隐藏面板；
no：显示面板。

示例：
``` 
<embed src="your.mid" hidden=ture>
<embed src="your.mid" hidden=no>
```
#### 4、开始时间
语法：starttime=mm:ss（分：秒）
说明：该属性规定音频或视频文件开始播放的时间。未定义则从文件开头播放。

示例：
```
<embed src="your.mid" starttime="00:10">
```
#### 5、音量大小
语法：volume=0-100之间的整数
说明：该属性规定音频或视频文件的音量大小。未定义则使用系统本身的设定。

示例：
```
<embed src="your.mid" volume="10">
```
#### 6、容器属性
语法：height=# width=#
说明：取值为正整数或百分数，单位为像素。该属性规定控制面板的高度和宽度。

height：控制面板的高度；
width：控制面板的宽度。

示例：
```
<embed src="your.mid" height=200 width=200>
```
#### 7、容器单位
语法：units=pixels、en
说明：该属性指定高和宽的单位为pixels或en。

示例：
```
<embed src="your.mid" units="pixels" height=200 width=200>
<embed src="your.mid" units="en" height=200 width=200>
```
#### 8、外观设置
语法：controls=console、smallconsole、playbutton、pausebutton、stopbutton、volumelever 说明：该属性规定控制面板的外观。默认值是console。
console：一般正常面板；
smallconsole：较小的面板；
playbutton：只显示播放按钮；
pausebutton：只显示暂停按钮；
stopbutton：只显示停止按钮；
volumelever：只显示音量调节按钮。

示例：
```
<embed src="your.mid" controls=smallconsole>
<embed src="your.mid" controls=volumelever>
```
#### 9、对象名称
语法：name=#
说明：#为对象的名称。该属性给对象取名，以便其他对象利用。

示例：
```
<embed src="your.mid" name="video">
```
#### 10、说明文字
语法：title=#
说明：#为说明的文字。该属性规定音频或视频文件的说明文字。

示例：
```
<embed src="your.mid" title="第一首歌">
```
#### 11、前景色和背景色
语法：palette=color|color
说明：该属性表示嵌入的音频或视频文件的前景色和背景色，第一个值为前景色，第二个值为背景色，中间用 | 隔开。color可以是RGB色（RRGGBB）也可以是颜色名，还可以是transparent （透明）。

示例：
```
<embed src="your.mid" palette="red|black">
```
#### 12、对齐方式
语法：align=top、bottom、center、baseline、 left、right、texttop、middle、absmiddle、absbottom
说明：该属性规定控制面板和当前行中的对象的对齐方式。

center：控制面板居中；
left：控制面板居左；
right：控制面板居右；
top：控制面板的顶部与当前行中的最高对象的顶部对齐；
bottom：控制面板的底部与当前行中的对象的基线对齐；
baseline：控制面板的底部与文本的基线对齐；
texttop：控制面板的顶部与当前行中的最高的文字顶部对齐；
middle：控制面板的中间与当前行的基线对齐；
absmiddle：控制面板的中间与当前文本或对象的中间对齐；
absbottom：控制面板的底部与文字的底部对齐。

示例：
```
<embed src="your.mid" align=top>
<embed src="your.mid" align=center>
```


## video

### 1、 定义和用法
`<video>` 标签定义视频，比如电影片段或其他视频流。
```
<video width="320" height="240" controls>
    <source src="movie.mp4" type="video/mp4">
    <source src="movie.ogg" type="video/ogg">
    您的浏览器不支持 video 标签。
</video>
```
### 2、标签定义及使用说明
目前，<video> 元素支持三种视频格式：MP4、WebM、Ogg。

| 浏览器            | MP4                                                     | WebM | Ogg  |
| :---------------- | :------------------------------------------------------ | :--- | :--- |
| Internet Explorer | YES                                                     | NO   | NO   |
| Chrome            | YES                                                     | YES  | YES  |
| Firefox           | YES 从 Firefox 21 版本开始 Linux 系统从 Firefox 30 开始 | YES  | YES  |
| Safari            | YES                                                     | NO   | NO   |
| Opera             | YES 从 Opera 25 版本开始                                | YES  | YES  |

- MP4 = MPEG 4文件使用 H264 视频编解码器和AAC音频编解码器

- WebM = WebM 文件使用 VP8 视频编解码器和 Vorbis 音频编解码器

- Ogg = Ogg 文件使用 Theora 视频编解码器和 Vorbis音频编解码器
### 3、属性

| 属性                                                         | 值       | 描述                                                         |
| :----------------------------------------------------------- | :------- | :----------------------------------------------------------- |
| autoplay | autoplay | 如果出现该属性，则视频在就绪后马上播放。                     |
| controls | controls | 如果出现该属性，则向用户显示控件，比如播放按钮。             |
| height | *pixels* | 设置视频播放器的高度。                                       |
| loop  | loop     | 如果出现该属性，则当媒介文件完成播放后再次开始播放。         |
| muted | muted    | 规定视频的音频输出应该被静音。                               |
| poster | *URL*    | 规定视频下载时显示的图像，或者在用户点击播放按钮前显示的图像。 |
| preload | preload  | 如果出现该属性，则视频在页面加载时进行加载，并预备播放。如果使用 "autoplay"，则忽略该属性。 |
| src | *url*    | 要播放的视频的 URL。                                         |
| width | *pixels* | 设置视频播放器的宽度。                                       |

### 4、使用DOM控制
HTML5 <video> 元素同样拥有方法、属性和事件。

其中的方法用于播放、暂停以及加载等。其中的属性（比如时长、音量等）可以被读取或设置。其中的 DOM 事件能够通知您，比方说，<video> 元素开始播放、已暂停，已停止，等等。

| 方法        | 属性        | 事件           |
| :---------- | :---------- | :------------- |
| play()      | currentSrc  | play           |
| pause()     | currentTime | pause          |
| load()      | videoWidth  | progress       |
| canPlayType | videoHeight | error          |
|             | duration    | timeupdate     |
|             | ended       | ended          |
|             | error       | abort          |
|             | paused      | empty          |
|             | muted       | emptied        |
|             | seeking     | waiting        |
|             | volume      | loadedmetadata |
|             | height      |                |
|             | width       |                |

**注释：**在所有属性中，只有 videoWidth 和 videoHeight 属性是立即可用的。在视频的元数据已加载后，其他属性才可用。

### 5、案例

**HTML5 视频播放器**

`index.html`

```
<!DOCTYPE html>
<html>
<head>
	<meta charset="UTF-8">
	<title>html5视频播放器</title>
	<link rel="stylesheet" href="./css/pure-min.css">
	<link rel="stylesheet" href="./css/main.css">
</head>
<body>
	<div class="wrapper">
		<div class="pure-g">
			<div class="pure-u-1">
				<div class="player">
					<video id="player" width="600" height="450">
						您的浏览器不支持HTML5
						<source src="./videos/echo-hereweare.mp4"></source>
					</video>
					<div class="pure-g" id="controller">
						<div class="pure-u-1-12">
							<span id="play" class="icon icon-play"></span>
							<span id="stop" class="icon icon-stop"></span>
						</div>
						<div class="pure-u-13-24 overflow-h">
							<div id="progressBar" class="controlBar">
								<div id="innerBar" class="controlInner"></div>
							</div>
						</div>
						<div class="pure-u-1-4">
							<span id="timer">0:00</span>
							<span id="volume" class="icon icon-volume"></span>
							<div id="volume-control" class="controlBar">
								<div id="volume-inner" class="controlInner"></div>
							</div>
						</div>
						<div class="pure-u-1-8 overflow-h">
							<span id="expand" class="icon icon-expand"></span>
							<span id="upload" class="icon icon-upload"></span>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div class="pure-g">
			<div class="pure-u-1">
				<input type="file" id="file">
			</div>
		</div>
	</div>
	<script src="./js/jquery-1.9.0.min.js"></script>
	<script src="./js/main.js"></script>
</body>
</html>
```
`main.js`

```
$(function(){
  var
    $player = $('#player'),
    $play = $('#play'),
    $stop = $('#stop'),
    $volume = $('#volume'),
    $expand = $('#expand'),
    $upload = $('#upload')

  var player = $player[0]

  var $timer = $('#timer'),
      $file = $('#file')

  var $innerBar = $('#innerBar'),
      $volumeControl = $('#volume-control'),
      $volumeInner = $('#volume-inner'),
      $progressBar = $('#progressBar')

  $play
    .on('click', function () {
      if (player.paused) {
        player.play()
        $(this).removeClass('icon-play').addClass('icon-pause')
      } else {
        player.pause()
        $(this).removeClass('icon-pause').addClass('icon-play')
      }
    })

  $stop
    .on('click', function () {
      player.currentTime = 0
      $innerBar.css('width', 0 + 'px')
      player.pause()
      $play.removeClass('icon-pause').addClass('icon-play')
    })

  $volume
    .on('click', function () {
      if (player.muted) {
        player.muted = false
        $(this).removeClass('icon-volume-mute').addClass('icon-volume')
        $volumeInner.css('width', 100 + '%')
      } else {
        player.muted = true
        $(this).removeClass('icon-volume').addClass('icon-volume-mute')
        $volumeInner.css('width', 0)
      }
    })

  $volumeControl
    .on('click', function (e) {
      var w = $(this).width(),
          x = e.offsetX

      window.vol = (x / w).toFixed(1) //全局变量

      player.volume = window.vol
      $volumeInner.css('width', x + 'px')
    })

  $progressBar
    .on('click', function (e) {
      var w = $(this).width(),
          x = e.offsetX
      window.per = (x / w).toFixed(3) //全局变量

      var duration = player.duration
      player.currentTime = (duration * window.per).toFixed(0)

      $innerBar.css('width', x + 'px')
    })

  $player
    .on('timeupdate', function () {
      // 秒数转换
      var time = player.currentTime.toFixed(1),
          minutes = Math.floor((time/60) % 60),
          seconds = Math.floor(time % 60)
      if (seconds < 10) {
        seconds = '0' + seconds
      }
      $timer.text(minutes + ':' + seconds)

      var w = $progressBar.width()
      if (player.duration) {
        var per = (player.currentTime / player.duration).toFixed(3)
        window.per = per
      } else {
        per = 0
      }
      $innerBar.css('width', (w * per).toFixed(0) + 'px')

      if (player.ended) { //播放完毕
        $play.removeClass('icon-pause').addClass('icon-play')
      }
    })

  $expand
    .on('click', function () {
      if (!document.webkitIsFullScreen) {
        player.webkitRequestFullScreen() //全屏
        $(this).removeClass('icon-expand').addClass('icon-contract')
      } else {
        document.webkitCancelFullScreen() //退出全屏
        $(this).removeClass('icon-contract').addClass('icon-expand')
      }
    })

  $upload
    .on('click', function () {
      $file.trigger('click')
    })

  $file
    .on('change', function (e) {
      var file = e.target.files[0],
          canPlayType = player.canPlayType(file.type)

      if (canPlayType === 'maybe' || canPlayType === 'probably') {
        var src = window.URL.createObjectURL(file)
        player.src = src
        $play.removeClass('icon-pause').addClass('icon-play')
        player.onload = function () {
          window.URL.revokeObjectURL(src)
        }
      } else {
        alert('浏览器不支持您选择的视频格式')
      }
    })
})
```



## audio

### 1、 定义和用法
`<audio>` 标签定义声音，比如音乐或其他音频流。
```
<audio src="someaudio.wav">
您的浏览器不支持 audio 标签。
</audio>
```

### 2、音频格式

当前，audio 元素支持三种音频格式：

|            | IE 9 | Firefox 3.5 | Opera 10.5 | Chrome 3.0 | Safari 3.0 |
| :--------- | :--- | :---------- | :--------- | :--------- | :--------- |
| Ogg Vorbis |      | √           | √          | √          |            |
| MP3        | √    |             |            | √          | √          |
| Wav        |      | √           | √          |            | √          |

### 3、属性

| 属性                | 描述                                                |
| :------------------ | :-------------------------------------------------- |
| audioTracks         | 返回表示可用音频轨道的 AudioTrackList 对象。        |
| autoplay            | 设置或返回是否在就绪（加载完成）后随即播放音频。    |
| buffered            | 返回表示音频已缓冲部分的 TimeRanges 对象。          |
| controller          | 返回表示音频当前媒体控制器的 MediaController 对象。 |
| controls            | 设置或返回音频是否应该显示控件（比如播放/暂停等）。 |
| crossOrigin         | 设置或返回音频的 CORS 设置。                        |
| currentSrc          | 返回当前音频的 URL。                                |
| currentTime         | 设置或返回音频中的当前播放位置（以秒计）。          |
| defaultMuted        | 设置或返回音频默认是否静音。                        |
| defaultPlaybackRate | 设置或返回音频的默认播放速度。                      |
| duration            | 返回音频的长度（以秒计）。                          |
| ended               | 返回音频的播放是否已结束。                          |
| error               | 返回表示音频错误状态的 MediaError 对象。            |
| loop                | 设置或返回音频是否应在结束时再次播放。              |
| mediaGroup          | 设置或返回音频所属媒介组合的名称。                  |
| muted               | 设置或返回是否关闭声音。                            |
| networkState        | 返回音频的当前网络状态。                            |
| paused              | 设置或返回音频是否暂停。                            |
| playbackRate        | 设置或返回音频播放的速度。                          |
| played              | 返回表示音频已播放部分的 TimeRanges 对象。          |
| preload             | 设置或返回音频的 preload 属性的值。                 |
| readyState          | 返回音频当前的就绪状态。                            |
| seekable            | 返回表示音频可寻址部分的 TimeRanges 对象。          |
| seeking             | 返回用户当前是否正在音频中进行查找。                |
| src                 | 设置或返回音频的 src 属性的值。                     |
| textTracks          | 返回表示可用文本轨道的 TextTrackList 对象。         |
| volume              | 设置或返回音频的音量。                              |

### 4、方法

| 方法           | 描述                                       |
| :------------- | :----------------------------------------- |
| addTextTrack() | 向音频添加新的文本轨道。                   |
| canPlayType()  | 检查浏览器是否能够播放指定的音频类型。     |
| fastSeek()     | 在音频播放器中指定播放时间。               |
| getStartDate() | 返回新的 Date 对象，表示当前时间线偏移量。 |
| load()         | 重新加载音频元素。                         |
| play()         | 开始播放音频。                             |
| pause()        | 暂停当前播放的音频。                       |

### 5、事件

play 播放事件 可判断歌曲是否正在播放中
pause 暂停事件 判断歌曲是否暂停
loadstart，durationchange，loadeddata，progress，canplay，canplaythrough。（这些事件在加载过程中是按以上顺序触发的）
以上这些事件可以通过事件监听对其做相应处理。

### 6、案例

**HTML5音乐播放器**
```
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<link rel="stylesheet" href="http://at.alicdn.com/t/font_1472646293_377639.css">
	<script src="js/jquery.js"></script>
	<style type="text/css">
		body{
			/*background: -webkit-linear-gradient(  ,#5621b8 0%,#781fa3 50%,#bc24b7 90%)*/
			background: -webkit-linear-gradient( right, #bc24b7 30%,#781fa3 50% ,#5621b8 80%)
		}
		p,ul,li{
			list-style: none;
			margin:0;
			padding: 0; 
		}
		#box{
			width: 1000px;
			height: 600px;
			/*border: 1px solid #000;*/
			position: absolute;
			top: 50%;
			left: 50%;
			margin-top: -300px;
			margin-left: -500px;
		}
		.top{
			height: 400px;
		}
		.pic-b{
			float: left;
			position: relative;
			width: 400px;
			height: 400px;
		}
		.picbg{
			
			width: 400px;
			height: 400px;
			background: url(img/cd.png) no-repeat center;
			background-size: 100%;
			border-radius: 50%;
			box-shadow: 1px 1px 15px #000;
			/*animation: active 3s linear infinite  .5s; */
		}
		@-webkit-keyframes active{
			from{
				-webkit-transform:rotate(0deg);
			}
			to{
				-webkit-transform:rotate(360deg);
			}
		}
		.pic{
			width: 200px;
			height: 200px;
			position: absolute;
			top: 50%;
			left: 50%;
			margin-left:-100px;
			margin-top: -100px;
			background: url(img/img.jpg)no-repeat center;
			background-size: 100%;
			border-radius: 50%;
		}
		.cdt{
			position: absolute;
			top: 0;
			right: -20px;
			/*background: url(img/cd_tou.png)no-repeat center;*/
			transform-origin: 60px 12px;
			transform: rotate(-21deg);
			-webkit-transition:all 1s;
		}
		.play{
			margin-top: 100px;
			width: 500px;
			float: right;
			font-family:"微软雅黑";
			color: #fff;
			text-align: center; 
			font-size: 18px;
		}
		/*.play2:visited{
			
		}*/
		.pl-c{
			margin-top: 20px;
			
		}
		.iconfont{
			color: #fff;
			cursor: pointer;
			font-size: 25px;
		}
		.pl-c-l{
			float: left;
			margin-left: 80px;
		}
		.pl-c-r{
			position: relative;	
			float: right;
			margin-right: 80px;
		}
		.pl-b{
			float: left;
		
			margin-left: 50px;

		}
		/*.pl-c-r .icon-1yinpinbofangmin{
			color：#eee;
		}*/
		/*.icon-1yinpinbofangmin:hover .vol{
			display: block;
		}*/
			.vol {
			display: none;
		    position: absolute;
		    width: 8px;
		    height: 100px;
		    top: -100px;
		    left: 70px;
		    background:  #E2D7D7;
		    border-radius: 15px;
		    border: 3px solid #fff;
		}
		.vol .vol1{
			position: absolute;
		    width: 8px;
		    height: 50px;
		    bottom: 0px;
		    left: 0px;
		    background:#EF6343;
		    border-radius: 4px;
		}
		.jindu{
			vertical-align: top;
			display: inline-block;
			margin-top: 12px;
			margin-left: 16px;
			width: 300px;
			height: 6px;
			border-radius: 1px;
			background: rgba(0,0,0,.4);
			position: relative;
			cursor: pointer;
		}
		.xxx{
			position: absolute;
			top: 0;
			left: 0;
			border-radius: 1px;
			background: #fff;
			height: 6px;
		}

		.center{
			width: 800px;
			margin: 80px auto;
			font-family: "微软雅黑"

		}
		.center li{
			text-align:center; 
			width: 162px;
			/*background:rgba(255,255,255,0.4);*/
			font-size: 27px;
			color: #fff;
			float: left;
			padding: 5px 5px 0 ;
			height: 75px;
			line-height: 40px;
			margin: 0 10px;
			border-radius: 8px;
			/*background: -webkit-linear-gradient(rgba(255,255,255,0.4) 46px,rgba(255,255,255,.1) 46px);*/
			position: relative;
			box-shadow: 2px 2px 4px rgba(0,0,0,.3);
			cursor: pointer;
		}
		.center li:hover{
			/*background: #000;*/
			-webkit-filter: blur(1px);
		}
		.center li:after{
			content: "";
			display: block;
			position: absolute;
			top: 0;
			left: 0;
			background: rgba(255,255,255,.3);
			border-radius: 8px 8px 0 0;
			width:100%;
			height: 50%;
			
		}
		.center li p{
			clear: both;
			font-size: 12px;
			line-height: 20px;
		}
		.center li b{
			font-size: 14px;
			
		}
	</style>
</head>
<body>
	<div id="box">
		<div class="top">
		  <div class="pic-b">
			<div class="picbg">
				<div class="pic"></div>
			</div>	
			<img class="cdt" src="img/cd_tou.png" />
		</div>
			<div class="play">
			  <div class="pl-t">
				<h1 style="font-size:50px;font-weight:normal">演员</h1>
				<span style="font-size:24px;">薛之谦</span>&nbsp;
				<span>专辑：绅士</span>
			  </div>
			  <div class="pl-c">
				   <div class="pl-c-l">
						 <span class="iconfont icon-back prev"></span>
						 <span class="iconfont icon-you-copy play2"></span>
						 <span class="iconfont icon-kuai next"></span>
					</div>
					<div class="pl-c-r">
						<span class="iconfont icon-suijibofang"></span>&nbsp;
						<span class="iconfont icon-zhongxinbofangicon"></span>&nbsp;
						<span class="iconfont icon-1yinpinbofangmin"></span>
						<div class="vol">
							<div class="vol1"></div>
						</div>
					</div>
					
					<div class="pl-b">
					<span class="time" style="font-size: 12px;">
						<n class="min1">00</n>:<n class="sec1">00</n>/<n class="min2">00</n>:<n class="sec2">00</n> 
					</span>
						<div class="jindu">
							<p class="xxx"></p>
						</div>
					</div>

			  </div>
			</div>
		</div>
		<ul class="center">
			<li>丑八怪<p><b>薛之谦</b><span>专题：绅士</span></p></li>
			<li>绅士<p><b>薛之谦</b><span>专题：绅士</span></p></li>
			<li>一半<p><b>薛之谦</b><span>专题：绅士</span></p></li>
			<li>认真的雪<p><b>薛之谦</b><span>专题：绅士</span></p></li>
		</ul>
	</div>
	<audio src="music/演员 - 薛之谦.mp3" type="audio/mp3" >
	 <!--  <source > -->
	</audio>
	<script>
		var audio=document.getElementsByTagName('audio')[0]; 
		var onoff=true;
		//  点击开关
		var onoff1=true; //音量开关
		var jindu;
		var weizhi;
		// var weiMin;
		// var weiSec;
		 function changeMusicActive(){
			clearTimeout(t2);
			rotateClear();
			$(".play2").removeClass('icon-you-copy');
			$(".play2").addClass('icon-zantingjian');
			onoff=false;
			//延时播放，以让它有重新播放的特效
			var t2=setTimeout(function(){
			$(".picbg").css('animation', ' active 3s linear infinite  .5s');
			$(".cdt").css('transform', 'rotate(0deg)');
			musicTime();   
			},500)
		}
		function musicStart(){
			audio.load();
			audio.play();
		}
		function musicTime(){	 
				var time=null;
				//歌曲时间
				 jindu=audio.duration;
				// var Jin=parseInt(jindu/60)<10 ? "0"+parseInt(jindu/60):parseInt(jindu/60);
				$('n.min2').text(parseInt(jindu/60));
				$('n.sec2').text(parseInt(jindu%60));
				
			}	
		function rotateClear(){
			$(".picbg").css('animation', '');  //清除旋转
			$(".cdt").css('transform', 'rotate(-21deg)');
		}
		var arrmusics=[["music/丑八怪 - 薛之谦.mp3","丑八怪"],["music/绅士 - 薛之谦.mp3","绅士"],["music/一半 - 薛之谦.mp3","一半"],["music/认真的雪 - 薛之谦.mp3","认真的雪"]];
		
		var $index=4;
	$(".center > li").click(function(){
		//先清除状态
		changeMusicActive();

		$index=$(this).index();
		audio.src=arrmusics[$index][0];
		$("h1").text(arrmusics[$index][1]);
		musicStart();
		// musicTime();   //写在这时间读不出来必须延迟等到加载完	
	})
	console.log($index);
	audio.addEventListener('timeupdate',function(){
		weizhi=audio.currentTime;
		var weiMin=parseInt(weizhi/60)<10 ? "0"+parseInt(weizhi/60):parseInt(weizhi/60);
		var  weiSec=parseInt(weizhi%60)<10 ? "0"+parseInt(weizhi%60):parseInt(weizhi%60);
		$('n.min1').text(weiMin);
		$('n.sec1').text(weiSec);
		var percent=audio.currentTime/audio.duration;
		// console.log(percent)
		$(".xxx").css('width', 300*percent);
		if (weizhi>=jindu) {
			rotateClear();
			$index++;
		if ($index>3) $index=0;
		audio.src=arrmusics[$index][0];
		$("h1").text(arrmusics[$index][1]);
		musicStart();
		changeMusicActive();
		}
	})
	//上一首
	
	$(".prev").click(function() {
		$index--;
		if ($index<0) $index=3;
		audio.src=arrmusics[$index][0];
		$("h1").text(arrmusics[$index][1]);
		musicStart();
		changeMusicActive();
	});
	//下一首
	$(".next").click(function() {
		$index++;
		if ($index>3) $index=0;
		audio.src=arrmusics[$index][0];
		$("h1").text(arrmusics[$index][1]);
		musicStart();
		changeMusicActive();
	});
    //随机播放键
    $('.icon-suijibofang').click(function(event) {
    	$index=Math.floor(Math.random()*4);
    	audio.src=arrmusics[$index][0];
    	$("h1").text(arrmusics[$index][1]);
		musicStart();
		changeMusicActive();
    });
	
	//进度移动
	$('.jindu').click(function(ev){
		ev=ev||event;
		var jindu_w=ev.clientX-$(".jindu").offset().left;  //offset如有定位的话返回的值为父级，否则相当于y值
		// console.log(parseInt(jindu_w/300*audio.duration));
		audio.currentTime=parseInt(jindu_w/300*audio.duration);

	})
	$(".play2").click(function() {
		jindu=0;
		weizhi=0;
	 	musicTime();
		
		if (onoff) {
			audio.play();
			// $(this).attr('class', 'iconfont icon-zantingjian play2');  两种换class名的方法
				$(this).removeClass('icon-you-copy');
				$(this).addClass('icon-zantingjian');
				//添加图画旋转
				$(".picbg").css('animation', ' active 3s linear infinite  .5s');
				$(".cdt").css('transform', 'rotate(0deg)');
		}else{
			audio.pause();
			$(this).removeClass('icon-zantingjian');
			$(this).addClass('icon-you-copy');
			rotateClear();
		}
		onoff=!onoff
	});

	//音量键的设置
	audio.volume=0.5;
	var t=null;
	$(".icon-1yinpinbofangmin").mouseover(function() {
		$(".vol").show();
	}).mouseout(function(event) {
		 t=setTimeout(function(){
		$(".vol").hide();
		},1000);
	});
	var volpast;
	$(".icon-1yinpinbofangmin").click(function() {
		
		//音量键点击一下静音
		if (onoff1) {
			volpast= $(".vol1").css('height');
			$(this).attr('class', 'iconfont icon-1');
		audio.volume=0;
		$(".vol1").css('height', 0);
		}else{   //再点击一下开音
			$(this).attr('class', 'iconfont icon-1yinpinbofangmin');
			audio.volume = parseInt(volpast)/100;
			console.log(audio.volume);
			$('.vol1').css('height', volpast);
		}
		onoff1=!onoff1;
	});
		$(".vol").mouseover(function(){	
			clearTimeout(t);
			$(this).show();
		}).mouseout(function(event) {

			$(this).hide();
		});
		//声音大小
		$(".vol").click(function(ev) {
			ev=ev||event;
			var volH=$('.vol').offset().top + 100 - event.clientY
			$(".vol1").css('height', volH);
			audio.volume=volH/100;
		});

		//重播
		$(".icon-zhongxinbofangicon").click(function(){
			musicStart();
		})

	</script>
</body>
</html>
```



## Canvas

### 0-1 canvas element

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Canvas Element</title>
</head>
<body>
  <canvas id="canvas" width="578" height="200"></canvas>
  <script>
    var canvas = document.getElementById('canvas')
    var context = canvas.getContext('2d')

    context.beginPath()
    context.moveTo(100, 150)
    context.lineTo(450, 50)
    context.stroke()
  </script>
</body>
</html>
```

### 1-1 line basic

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Line Basic</title>
</head>
<body>
  <canvas id="canvas" width="578" height="200"></canvas>
  <script>
    var canvas = document.getElementById('canvas')
    var context = canvas.getContext('2d')

    context.beginPath()
    context.moveTo(100, 150)
    context.lineTo(450, 50)

    context.strokeStyle = '#ff0000'
    context.lineWidth = 15
    context.stroke()
  </script>
</body>
</html>
```

### 1-2 line cap	

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Line cap</title>
</head>
<body>
  <canvas id="canvas" width="578" height="200"></canvas>
  <script>
    var canvas = document.getElementById('canvas')
    var context = canvas.getContext('2d')

    context.beginPath()
    context.moveTo(200, canvas.height / 2 - 50)
    context.lineTo(canvas.width - 200, canvas.height / 2 - 50)
    context.lineWidth = 20;
    context.strokeStyle = '#0000ff'
    context.lineCap = 'butt'
    context.stroke()

    context.beginPath()
    context.moveTo(200, canvas.height / 2)
    context.lineTo(canvas.width - 200, canvas.height / 2)
    context.lineWidth = 20;
    context.strokeStyle = '#0000ff'
    context.lineCap = 'round'
    context.stroke()

    context.beginPath()
    context.moveTo(200, canvas.height / 2  + 50)
    context.lineTo(canvas.width - 200, canvas.height / 2 + 50)
    context.lineWidth = 20;
    context.strokeStyle = '#0000ff'
    context.lineCap = 'square'
    context.stroke()
  </script>
</body>
</html>
```

### 2-1 arc

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Arc</title>
</head>
<body>
  <canvas id="canvas" width="578" height="200"></canvas>
  <script>
    var canvas = document.getElementById('canvas')
    var context = canvas.getContext('2d')

    var x = canvas.width / 2
    var y = canvas.height / 2
    var radius = 75
    var startAngle = 1.1 * Math.PI
    var endAngle = 1.9 * Math.PI
    var counterClockwise = false

    context.beginPath()
    context.arc(x, y, radius, startAngle, endAngle, counterClockwise)

    context.strockStyle = 'black'
    context.stroke()
  </script>
</body>
</html>
```

### 2-2 quadratic curve：二次曲线

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Quadratic curve</title>
</head>
<body>
  <canvas id="canvas" width="578" height="200"></canvas>
  <script>
    var canvas = document.getElementById('canvas');
    var context = canvas.getContext('2d');

    context.beginPath()
    context.moveTo(188, 150)
    context.quadraticCurveTo(188, 0, 488, 150)
    context.lineWidth = 10

    context.strokeStyle = 'black'
    context.stroke()
  </script>
</body>
</html>
```

### 2-3 bezier curve : 三次贝塞尔曲线

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Bezier curve</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.moveTo(188, 130)
      context.bezierCurveTo(140, 10, 288, 10, 388, 170)

      context.lineWidth = 10
      context.strokeStyle = 'black'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 3-1 path

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Path</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.moveTo(100, 20)

      context.lineTo(200, 160)

      context.quadraticCurveTo(230, 200, 250, 120)

      context.bezierCurveTo(290, -40, 300, 200, 400, 150)

      context.lineTo(500, 90)

      context.lineWidth = 5
      context.strokeStyle = 'blue'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 3-2 path join

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Path join</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.lineWidth = 25

      context.beginPath()
      context.moveTo(99, 150)
      context.lineTo(149, 50)
      context.lineTo(199, 150)
      context.lineJoin = 'miter'
      context.stroke()

      context.beginPath()
      context.moveTo(239, 150)
      context.lineTo(289, 50)
      context.lineTo(339, 150)
      context.lineJoin = 'round'
      context.stroke()

      context.beginPath()
      context.moveTo(379, 150)
      context.lineTo(429, 50)
      context.lineTo(479, 150)
      context.lineJoin = 'bevel'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 3-3 rounded corners

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>rounded corners</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.lineWidth = 25

      context.beginPath()
      context.moveTo(99, 150)
      context.lineTo(149, 50)
      context.lineTo(199, 150)
      context.lineJoin = 'miter'
      context.stroke()

      context.beginPath()
      context.moveTo(239, 150)
      context.lineTo(289, 50)
      context.lineTo(339, 150)
      context.lineJoin = 'round'
      context.stroke()

      context.beginPath()
      context.moveTo(379, 150)
      context.lineTo(429, 50)
      context.lineTo(479, 150)
      context.lineJoin = 'bevel'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 4-1 custom shape

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>custom shape</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.moveTo(170, 80)
      context.bezierCurveTo(130, 100, 130, 150, 230, 150)
      context.bezierCurveTo(250, 180, 320, 180, 340, 150)
      context.bezierCurveTo(420, 150, 420, 120, 390, 100)
      context.bezierCurveTo(430, 40, 370, 30, 340, 50)
      context.bezierCurveTo(320, 5, 250, 20, 250, 50)
      context.bezierCurveTo(200, 5, 150, 20, 170, 80)

      context.closePath()
      context.lineWidth = 5
      context.strokeStyle = 'blue'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 4-2 rectangle

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>rectangle</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.rect(188, 50, 200, 100)

      context.fillStyle = 'yellow'
      context.fill()

      context.lineWidth = 7
      context.strokeStyle = 'black'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 4-3 circle

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>circle</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var centerX = canvas.width / 2
      var centerY = canvas.height / 2
      var radius = 70

      context.beginPath()
      context.arc(centerX, centerY, radius, 0, 2 * Math.PI, false)
      context.fillStyle = 'green'
      context.fill()
      context.lineWidth = 5
      context.strokeStyle = '#003300'
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 4-4 semicircle

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>semicircle</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.arc(288, 75, 70, 0, Math.PI, false)
      context.closePath()

      context.lineWidth = 5
      context.fillStyle = 'red'
      context.strokeStyle = '#550000'

      context.fill()
      context.stroke()
    </script>
  </script>
</body>
</html>
```

### 5-1 color fill

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>color fill</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.beginPath()
      context.moveTo(170, 80)
      context.bezierCurveTo(130, 100, 130, 150, 230, 150)
      context.bezierCurveTo(250, 180, 320, 180, 340, 150)
      context.bezierCurveTo(420, 150, 420, 120, 390, 100)
      context.bezierCurveTo(430, 40, 370, 30, 340, 50)
      context.bezierCurveTo(320, 5, 250, 20, 250, 50)
      context.bezierCurveTo(200, 5, 150, 20, 170, 80)

      context.closePath()
      context.lineWidth = 5
      context.strokeStyle = 'blue'
      context.stroke()
      context.fillStyle = 'red'
      context.fill()
    </script>
  </script>
</body>
</html>
```

### 5-2 linear gradient

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>linear gradient</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.rect(0, 0, canvas.width, canvas.height)

      var grd = context.createLinearGradient(0, 0, canvas.width, canvas.height)
      grd.addColorStop(0, '#8ED6FF')
      grd.addColorStop(1, '#004CB3')

      context.fillStyle = grd
      context.fill()
    </script>
  </script>
</body>
</html>
```

### 5-3 radial gradient

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>radial gradient</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.rect(0, 0, canvas.width, canvas.height)

      var grd = context.createRadialGradient(238, 50, 10, 238, 50, 300)
      grd.addColorStop(0, '#8ED6FF')
      grd.addColorStop(1, '#004CB3')
      context.fillStyle = grd
      context.fill()
    </script>
  </script>
</body>
</html>
```

### 5-4 pattern

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>pattern</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var imageObj = new Image()
      imageObj.src = './wood-pattern.png'
      imageObj.onload = function() {
        var pattern = context.createPattern(imageObj, 'repeat')

        context.rect(0, 0, canvas.width, canvas.height)
        context.fillStyle = pattern
        context.fill()
      }
    </script>
  </script>
</body>
</html>
```

### 6-1 draw image

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>draw image</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var imageObj = new Image()
      imageObj.src = './darth-vader.jpg'
      imageObj.onload = function() {
        context.drawImage(imageObj, 69, 50)
      }
    </script>
  </script>
</body>
</html>
```

### 6-2 image size

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>image size</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var x = 188
      var y = 30
      var width = 438
      var height = 300

      var imageObj = new Image()
      imageObj.src = './darth-vader.jpg'
      imageObj.onload = function() {
        context.drawImage(imageObj, x, y, width, height)
      }
    </script>
  </script>
</body>
</html>
```

### 6-3 image crop

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>image crop</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var sourceX = 100
      var sourceY = 10
      var sourceWidth = 250
      var sourceHeight = 250

      var destWidth = sourceWidth
      var destHeight = sourceHeight
      var destX = canvas.width / 2 - destWidth / 2
      var destY = canvas.height / 2 - destHeight / 2

      var imageObj = new Image()
      imageObj.src = './darth-vader.jpg'
      imageObj.onload = function() {
        context.drawImage(imageObj, sourceX, sourceY, sourceWidth, sourceHeight, 100, 100, destWidth, destHeight)
      }
    </script>
  </script>
</body>
</html>
```

### 6-4 image loader

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>image loader</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var sources = {
        darthVader: './darth-vader.jpg',
        yoda: './yoda.jpg'
      }

      function loadImages(sources, callback) {
        var images = {}
        var loadedImages = 0
        var numImages = 0

        for(var src in sources) {
          numImages++
        }

        for(var src in sources) {
          images[src] = new Image()
          images[src].onload = function() {
            if(++loadedImages >= numImages) {
              callback(images)
            }
          }
          images[src].src = sources[src]
        }
      }

      loadImages(sources, function(images){
        context.drawImage(images.darthVader, 100, 30, 200, 137)
        context.drawImage(images.yoda, 350, 55, 93, 104)
      })
    </script>
</body>
</html>
```

### 7-1 text basic

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>text basic</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var text = 'Hello World'

      var x = canvas.width / 2
      var y = canvas.height / 2

      context.font = 'bold 20pt Calibri'
      context.fillStyle = 'blue'

      context.textAlign = 'center' // start end left right
      context.textBaseline = 'middle' //top hanging alphabetic bottom

      var metrics = context.measureText(text)
      var width = metrics.width

      context.fillText('(' + width + 'px wide)', x, y)

      // context.strokeStyle = 'red'
      // context.strokeText('Hello World', 150, 100)
    </script>
</body>
</html>
```

### 7-2 text wrap

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>text wrap</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var maxWidth = 400
      var lineHeight = 25
      var x = (canvas.width - maxWidth) / 2
      var y = 60
      var text = 'All the world \'s a stage, and all the men and women merely players. They have their exits and their entrances; And one man in his time plays many parts.'

      context.font = '16pt Calibri'
      context.fillStyle = '#333'

      function wrapText(context, text, x, y, maxWidth, lineHeight) {
        var words = text.split(' ')
        var line = ''

        for(var n = 0; n < words.length; n++) {
          var textLine = line + words[n] + ' '
          var metrics = context.measureText(textLine)
          var textWidth = metrics.width
          if (textWidth > maxWidth && n > 0) {
            context.fillText(line, x, y)
            line = words[n] + ' '
            y += lineHeight
          } else {
            line = textLine
          }
        }

        context.fillText(line, x, y)
      }

      wrapText(context, text, x, y, maxWidth, lineHeight)
    </script>
</body>
</html>
```

### 8-1 translate

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>translate</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWidth = 150
      var rectHeight = 75

      context.translate(canvas.width / 2, canvas.height / 2)

      context.fillStyle = 'blue'
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight)
    </script>
</body>
</html>
```

### 8-2 scale

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>scale</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWidth = 150
      var rectHeight = 75

      context.translate(canvas.width / 2, canvas.height / 2)

      context.scale(2, 2)

      context.fillStyle = 'blue'
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight)
    </script>
</body>
</html>
```

### 8-3 rotate

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>rotate</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWidth = 150
      var rectHeight = 75

      context.translate(canvas.width / 2, canvas.height / 2)

      context.rotate(Math.PI/4)

      context.fillStyle = 'blue'
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight)
    </script>
</body>
</html>
```

### 8-4 custom transform

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>custom transform</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWidth = 150
      var rectHeight = 75

      // transform matrix
      // a c e
      // b d f
      // 0 0 1

      // 平移
      // 1 0 x
      // 0 1 y
      // 0 0 1

      // 缩放
      // x 0 0
      // 0 y 0
      // 0 0 1

      // 旋转
      // cos(x) -sin(x) 0
      // sin(x) cos(x)  0
      // 0      0       1

      // 变形
      // 1      tan(y) 0
      // tan(x) 1      0
      // 0      0      1

      var rectWidth = 150
      var rectHeight = 75

      var x = canvas.width / 2
      var y = canvas.height / 2

      context.transform(1, 0, 0, 1, x, y)

      // context.rotate(Math.PI/4)
      context.transform(Math.cos(Math.PI/4), Math.sin(Math.PI/4), -Math.sin(Math.PI/4), Math.cos(Math.PI/4), 0, 0)

      // context.transform(2, 0, 0, 2, 0, 0)

      context.fillStyle = 'blue'
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight)
    </script>
</body>
</html>
```

### 8-5 mirror

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>mirror</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.translate(canvas.width/2, canvas.height/2)

      context.scale(-1, 1)

      context.font = '30pt Calibri'
      context.textAlign = 'center'
      context.fillStyle = 'blue'
      context.fillText('Hello World', 0, 0)
    </script>
</body>
</html>
```

### 8-6 reset transform

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>reset transform</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="200"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWith = 150
      var rectHeight = 75

      context.translate(canvas.width / 2, canvas.height / 2)
      context.fillStyle = 'blue'
      context.fillRect(-rectWith /2, rectHeight / -2, rectWith, rectHeight)

      // reset transform
      // 1 0 0
      // 0 1 0
      // 0 0 1
      // context.setTransform(1, 0, 0, 1, 0, 0)
      context.fillStyle = 'red'
      context.fillRect(0, 0, rectWith, rectHeight)
    </script>
</body>
</html>
```

### 8-7 state stack

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>state stack</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var rectWidth = 150
      var rectHeight = 75

      context.save()
      context.translate(canvas.width / 2, canvas.height / 2);

      context.save()
      context.rotate(Math.PI / 4);

      context.save()
      context.scale(2, 2);

      context.fillStyle = 'blue';
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight);
      context.restore()

      context.fillStyle = 'red';
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight);
      context.restore()

      context.fillStyle = 'yellow';
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight);
      context.restore()
      
      context.fillStyle = 'green';
      context.fillRect(rectWidth / -2, rectHeight / -2, rectWidth, rectHeight);

    </script>
</body>
</html>
```

### 8-8 oval

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>oval</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var centerX = 0
      var centerY = 0
      var radius = 50

      context.save()
      context.translate(canvas.width/2, canvas.height/2)

      context.scale(2, 1)

      context.beginPath()
      context.arc(centerX, centerY, radius, 0, 2*Math.PI, false)

      context.restore()

      context.fillStyle = '#8ED6FF'
      context.fill()
      context.lineWidth = 5
      context.strokeStyle = 'black'
      context.stroke()

    </script>
</body>
</html>
```

### 9-1 shadow

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>shadow</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.rect(188, 40, 200, 100)
      context.fillStyle = 'red'
      context.shadowColor = '#999'
      context.shadowBlur = 20
      context.shadowOffsetX = 15
      context.shadowOffsetY = 15
      context.fill()

    </script>
</body>
</html>
```

### 9-2 global alpha

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>global alpha</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      context.globalAlpha = 0.1
      context.beginPath()
      context.rect(200, 20, 100, 100)
      context.fillStyle = 'blue'
      context.fill()

      context.globalAlpha = 0.5
      context.beginPath()
      context.arc(320, 120, 60, 0, 2 * Math.PI, false)
      context.fillStyle = 'red'
      context.fill()

    </script>
</body>
</html>
```

### 9-3 clipping region

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>clipping region</title>
</head>
<body>
    <canvas id="myCanvas" width="578" height="400"></canvas>
    <script>
      var canvas = document.getElementById('myCanvas');
      var context = canvas.getContext('2d');

      var x = canvas.width / 2
      var y = canvas.height / 2
      var radius = 75
      var offset = 50

      context.save();
      context.beginPath()
      context.arc(x, y, radius, 0, 2 * Math.PI, false)
      context.clip()

      context.beginPath()
      context.arc(x - offset, y - offset, radius, 0, 2 * Math.PI, false)
      context.fillStyle = 'blue'
      context.fill()

      context.beginPath()
      context.arc(x + offset, y, radius, 0, 2 * Math.PI, false)
      context.fillStyle = 'yellow'
      context.fill()

      context.beginPath()
      context.arc(x, y + offset, radius, 0, 2 * Math.PI, false)
      context.fillStyle = 'red'
      context.fill()

      context.restore()
      context.beginPath()
      context.arc(x, y, radius, 0, 2 * Math.PI, false)
      context.lineWidth = 10
      context.strokeStyle = 'purple'
      context.stroke()

    </script>
</body>
</html>
```

### 9-4 operations

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>operations</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <canvas id="tempCanvas" width="578" height="430" style="display:none"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');
    var tempCanvas = document.getElementById('tempCanvas')
    var tempContext = tempCanvas.getContext('2d')

    var squareWidth = 55
    var circleRadius = 35
    var shapeOffset = 50
    var operationOffset = 150
    var arr = []

    arr.push('source-atop')
    arr.push('source-in')
    arr.push('source-out')
    arr.push('source-over')
    arr.push('destination-atop')
    arr.push('destination-in')
    arr.push('destination-out')
    arr.push('destination-over')
    arr.push('lighter')
    arr.push('darker')
    arr.push('xor')
    arr.push('copy')

    context.translate(10, 10)
    for (var n = 0; n < arr.length; n++) {
      var thisOperation = arr[n]

      tempContext.save()
      tempContext.clearRect(0, 0, canvas.width, canvas.height)

      tempContext.beginPath()
      tempContext.rect(0, 0, squareWidth, squareWidth)
      tempContext.fillStyle = 'blue'
      tempContext.fill()

      tempContext.globalCompositeOperation = thisOperation

      tempContext.beginPath()
      tempContext.arc(shapeOffset, shapeOffset, circleRadius, 0, 2 * Math.PI, false)
      tempContext.fillStyle = 'red'
      tempContext.fill()
      tempContext.restore()

      tempContext.font = '10pt Verdana'
      tempContext.fillStyle = 'black'
      tempContext.fillText(thisOperation, 0, squareWidth + 45)

      if (n > 0) {
        if (n % 4 === 0) {
          context.translate(operationOffset * -3, operationOffset)
        } else {
          context.translate(operationOffset, 0)
        }
      }

      context.drawImage(tempCanvas, 0, 0)
    }
  </script>
</body>
</html>
```

### 10-1 image data

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>image data</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');
    var imageObj = new Image()
    imageObj.onload = function () {
      drawImage(this)
    }
    imageObj.src = './darth-vader.jpg'

    function drawImage(imageObj) {
      var imageX = 69
      var imageY = 50
      var imageWidth = imageObj.width
      var imageHeight = imageObj.height
      context.drawImage(imageObj, imageX, imageY)

      var imageData = context.getImageData(imageX, imageY, imageWidth, imageHeight)
      var data = imageData.data

      for (var i = 0; i < data.length; i++) {
        var red = data[i]
        var green = data[i + 1]
        var blue = data[i + 2]
        var alpha = data[i + 3]
      }
    }
  </script>
</body>
</html>
```

### 10-2 invert colors

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>invert colors</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    var imageObj = new Image()
    imageObj.onload = function () {
      drawImage(this)
    }
    imageObj.src = './darth-vader.jpg'

    function drawImage(imageObj) {
      var x = 69
      var y = 50

      context.drawImage(imageObj, x, y)

      var imageData = context.getImageData(x, y, imageObj.width, imageObj.height)
      var data = imageData.data

      for (var i = 0; i < data.length; i += 4) {
        data[i] = 255 - data[i]
        data[i + 1] = 255 - data[i + 1]
        data[i + 2] = 255 - data[i + 2]
      }

      context.putImageData(imageData, x, y)
    }
  </script>
</body>
</html>
```

### 10-3 grayscale

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>grayscale</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    var imageObj = new Image()
    imageObj.onload = function () {
      drawImage(this)
    }
    imageObj.src = './darth-vader.jpg'

    function drawImage(imageObj) {
      var x = 69
      var y = 50

      context.drawImage(imageObj, x, y)

      var imageData = context.getImageData(x, y, imageObj.width, imageObj.height)
      var data = imageData.data

      for (var i = 0; i < data.length; i += 4) {
        var brightness = 0.34 * data[i] + 0.5 * data[i + 1] + 0.16 * data[i + 2]
        data[i] = brightness
        data[i + 1] = brightness
        data[i + 2] = brightness
      }

      context.putImageData(imageData, x, y)
    }
  </script>
</body>
</html>
```

### 10-4 get data url

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>get data url</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    context.beginPath()
    context.moveTo(170, 80)
    context.bezierCurveTo(130, 100, 130, 150, 230, 150)
    context.bezierCurveTo(250, 180, 320, 180, 340, 150)
    context.bezierCurveTo(420, 150, 420, 120, 390, 100)
    context.bezierCurveTo(430, 40, 370, 30, 340, 50)
    context.bezierCurveTo(320, 5, 250, 20, 250, 50)
    context.bezierCurveTo(200, 5, 150, 20, 170, 80)

    context.closePath()
    context.lineWidth = 10
    context.strokeStyle = '#0000ff'
    context.stroke()
    context.fillStyle = '#8ED6FF'
    context.fill()

    var dataURL = canvas.toDataURL()
    console.log(dataURL)
  </script>
</body>
</html>
```

### 10-5 load data url

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>load data url</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    var request = new XMLHttpRequest()
    request.open('GET', './dataURL.txt', true)
    request.onreadystatechange = function () {
      if (request.readyState == 4) {
        if (request.status == 200) {
          loadCanvas(request.responseText)
        }
      }
    }
    request.send(null)

    function loadCanvas(dataURL) {
      var imageObj = new Image()
      imageObj.onload = function () {
        context.drawImage(this, 0, 0)
      }
      imageObj.src = dataURL
    }
  </script>
</body>
</html>
```

### 10-6 save drawing

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>save drawing</title>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430" style="display:none"></canvas>
  <img src="" id="canvasImg" alt="">
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    context.beginPath()
    context.moveTo(170, 80)
    context.bezierCurveTo(130, 100, 130, 150, 230, 150)
    context.bezierCurveTo(250, 180, 320, 180, 340, 150)
    context.bezierCurveTo(420, 150, 420, 120, 390, 100)
    context.bezierCurveTo(430, 40, 370, 30, 340, 50)
    context.bezierCurveTo(320, 5, 250, 20, 250, 50)
    context.bezierCurveTo(200, 5, 150, 20, 170, 80)

    context.closePath()
    context.lineWidth = 10
    context.strokeStyle = '#0000ff'
    context.stroke()
    context.fillStyle = '#8ED6FF'
    context.fill()

    var dataURL = canvas.toDataURL()
    document.getElementById('canvasImg').src = dataURL
  </script>
</body>
</html>
```

### 11-1 clear canvas

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>clear canvas</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
    #buttons {
      position: absolute;
      top: 5px;
      left: 10px;
    }
    #buttons > input {
      padding: 10px;
      display: block;
      margin-top: 5px;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <div id="buttons">
    <input type="button" id="clear" name="" value="Clear">
  </div>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    context.beginPath()
    context.moveTo(170, 80)
    context.bezierCurveTo(130, 100, 130, 150, 230, 150)
    context.bezierCurveTo(250, 180, 320, 180, 340, 150)
    context.bezierCurveTo(420, 150, 420, 120, 390, 100)
    context.bezierCurveTo(430, 40, 370, 30, 340, 50)
    context.bezierCurveTo(320, 5, 250, 20, 250, 50)
    context.bezierCurveTo(200, 5, 150, 20, 170, 80)

    context.closePath()
    context.lineWidth = 10
    context.strokeStyle = '#0000ff'
    context.stroke()
    context.fillStyle = '#8ED6FF'
    context.fill()

    document.getElementById('clear').addEventListener('click', function () {
      context.clearRect(0, 0, canvas.width, canvas.height)
    })
  </script>
</body>
</html>
```

### 11-2 animation clears

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>animation clears</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    window.requestAnimFrame = (function (callback) {
      return window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(callback) {
        window.setTimeout(callback, 1000 / 60)
      }
    })()

    function drawRectangle(myRectangle, context) {
      context.beginPath()
      context.rect(myRectangle.x, myRectangle.y, myRectangle.width, myRectangle.height)
      context.fillStyle = '#8ED6FF'
      context.fill()
      context.lineWidth = myRectangle.borderWidth
      context.strokeStyle = 'black'
      context.stroke()
    }

    function animate(myRectangle, canvas, context, startTime) {
      var time = (new Date()).getTime() - startTime
      var linearSpeed = 100
      var newX = linearSpeed * time / 1000
      if (newX < canvas.width - myRectangle.width - myRectangle.borderWidth / 2) {
        myRectangle.x = newX
      }
      context.clearRect(0, 0, canvas.width, canvas.height)

      drawRectangle(myRectangle, context)

      requestAnimFrame(function () {
        animate(myRectangle, canvas, context, startTime)
      })
    }

    var myRectangle = {
      x: 0,
      y: 75,
      height: 50,
      width: 100,
      borderWidth: 5
    }

    drawRectangle(myRectangle, context)

    setTimeout(function () {
      var startTime = (new Date()).getTime()
      animate(myRectangle, canvas, context, startTime)
    }, 1000)
  </script>
</body>
</html>
```

### 11-3 acceleration

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>acceleration</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    window.requestAnimFrame = (function (callback) {
      return window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(callback) {
        window.setTimeout(callback, 1000 / 60)
      }
    })()

    function drawRectangle(myRectangle, context) {
      context.beginPath()
      context.rect(myRectangle.x, myRectangle.y, myRectangle.width, myRectangle.height)
      context.fillStyle = '#8ED6FF'
      context.fill()
      context.lineWidth = myRectangle.borderWidth
      context.strokeStyle = 'black'
      context.stroke()
    }

    function animate(myRectangle, canvas, context, startTime) {
      var time = (new Date()).getTime() - startTime

      var gravity = 200

      myRectangle.y = 0.5 * gravity * Math.pow(time / 1000, 2)

      if (myRectangle.y > canvas.height - myRectangle.height - myRectangle.borderWidth / 2) {
        myRectangle.y = canvas.height - myRectangle.height - myRectangle.borderWidth / 2
      }
      lastTime = time

      context.clearRect(0, 0, canvas.width, canvas.height)

      drawRectangle(myRectangle, context)

      requestAnimFrame(function () {
        animate(myRectangle, canvas, context, startTime)
      })
    }

    var myRectangle = {
      x: 0,
      y: 75,
      height: 50,
      width: 100,
      borderWidth: 5
    }

    drawRectangle(myRectangle, context)

    setTimeout(function () {
      var startTime = (new Date()).getTime()
      animate(myRectangle, canvas, context, startTime)
    }, 1000)
  </script>
</body>
</html>
```

### 11-4 oscillation

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>oscillation</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    window.requestAnimFrame = (function (callback) {
      return window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(callback) {
        window.setTimeout(callback, 1000 / 60)
      }
    })()

    function drawRectangle(myRectangle, context) {
      context.beginPath()
      context.rect(myRectangle.x, myRectangle.y, myRectangle.width, myRectangle.height)
      context.fillStyle = '#8ED6FF'
      context.fill()
      context.lineWidth = myRectangle.borderWidth
      context.strokeStyle = 'black'
      context.stroke()
    }

    function animate(myRectangle, canvas, context, startTime) {
      var time = (new Date()).getTime() - startTime

      var amplitude = 150
      var period = 2000
      var centerx = canvas.width / 2 - myRectangle.width / 2
      var nextX = amplitude * Math.sin(time * 2 * Math.PI / period) + centerx
      myRectangle.x = nextX

      context.clearRect(0, 0, canvas.width, canvas.height)

      drawRectangle(myRectangle, context)

      requestAnimFrame(function () {
        animate(myRectangle, canvas, context, startTime)
      })
    }

    var myRectangle = {
      x: 0,
      y: 75,
      height: 50,
      width: 100,
      borderWidth: 5
    }

    drawRectangle(myRectangle, context)

    setTimeout(function () {
      var startTime = (new Date()).getTime()
      animate(myRectangle, canvas, context, startTime)
    }, 1000)
  </script>
</body>
</html>
```

### 11-5 start and stop

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>start and stop</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    window.requestAnimFrame = (function (callback) {
      return window.requestAnimationFrame || window.webkitRequestAnimationFrame || window.mozRequestAnimationFrame || window.oRequestAnimationFrame || window.msRequestAnimationFrame || function(callback) {
        window.setTimeout(callback, 1000 / 60)
      }
    })()

    function drawRectangle(myRectangle, context) {
      context.beginPath()
      context.rect(myRectangle.x, myRectangle.y, myRectangle.width, myRectangle.height)
      context.fillStyle = '#8ED6FF'
      context.fill()
      context.lineWidth = myRectangle.borderWidth
      context.strokeStyle = 'black'
      context.stroke()
    }

    function animate(myRectangle, canvas, context, startTime, runAnimation) {
      if (runAnimation.value) {
        var time = (new Date()).getTime() - startTime

        var amplitude = 150
        var period = 2000
        var centerx = canvas.width / 2 - myRectangle.width / 2
        var nextX = amplitude * Math.sin(time * 2 * Math.PI / period) + centerx
        myRectangle.x = nextX

        context.clearRect(0, 0, canvas.width, canvas.height)

        drawRectangle(myRectangle, context)

        requestAnimFrame(function () {
          animate(myRectangle, canvas, context, startTime, runAnimation)
        })
      }
    }

    var myRectangle = {
      x: 0,
      y: 75,
      height: 50,
      width: 100,
      borderWidth: 5
    }

    var runAnimation = {
      value: false
    }

    document.getElementById('myCanvas').addEventListener('click', function () {
      runAnimation.value = !runAnimation.value
      if (runAnimation.value) {
        var startTime = (new Date()).getTime()
        animate(myRectangle, canvas, context, startTime, runAnimation)
      }
    })

    drawRectangle(myRectangle, context)
  </script>
</body>
</html>
```

### 12-1 mouse coordinates

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>mouse coordinates</title>
  <style media="screen">
    body {
      margin: 0;
      padding: 0;
    }
  </style>
</head>
<body>
  <canvas id="myCanvas" width="578" height="430"></canvas>
  <script>
    var canvas = document.getElementById('myCanvas');
    var context = canvas.getContext('2d');

    function getMousePos(canvas, evt) {
      var rect = canvas.getBoundingClientRect()
      return {
        x: evt.clientX - rect.left,
        y: evt.clientY - rect.top
      }
    }

    function writeMessage(canvas, message) {
      context.clearRect(0, 0, canvas.width, canvas.height)
      context.font = '18pt Calibri'
      context.fillStyle = 'black'
      context.fillText(message, 10, 25)
    }

    canvas.addEventListener('mousemove', function (evt) {
      var mousePos = getMousePos(canvas, evt)
      var message = 'Mouse position:' + mousePos.x + ',' + mousePos.y
      writeMessage(canvas, message)
    }, false)
  </script>
</body>
</html>
```

### 案例赏析

![image-20190526101518932](/Users/Felix/Library/Application Support/typora-user-images/image-20190526101518932.png)

![image-20190526101536122](/Users/Felix/Library/Application Support/typora-user-images/image-20190526101536122.png)

![image-20190526101557611](/Users/Felix/Library/Application Support/typora-user-images/image-20190526101557611.png)

![image-20190526101620638](/Users/Felix/Library/Application Support/typora-user-images/image-20190526101620638.png)



## 本地存储

### Web Storage 简介
Web Storage 可以让应用在用户的本地上存储一些内容，这些内容是成对出现的，内容的名称，还有内容的具体的值。使用 setItem ，可以去设置存储的内容，然后用 getItem 可以获取到存储的具体的内容。

Web Storage 分成两个部分 Local Storage ，还有 Session Storage ，他们的用法基本上是一样的，有点不同的是，Local Storage 存储的东西在关掉浏览器的时候不会消失。

Session Storage 的数据在关掉浏览器的时候，会自动清除掉。
### Local Storage
#### Local Storage - 在浏览器中存储数据
```
localStorage.setItem('name', '好程序员')
```
在Chrome浏览器的Application/Storage/Local Storage 查看内容
重新设置值：

```
localStorage.setItem('name', 'gp')
```
#### 获取存储在浏览器中的 Local Storage 数据

```
localStorage.getItem('name') // gp
localStorage.length // 1
localStorage.setItem('birthTime', '2016-08')
localStorage.length // 2
```

#### 移除存储在浏览器中的 Local Storage 数据

```
localStorage.removeItem('name')
localStorage.getItem('name') // null
localStorage.clear()
```

### 事件

#### Storage 事件

当存储区域发生变化的时候，会触发一个 storage 事件。比如设置新的数据，移除或者清除数据的时候，都会触发这个 storage 事件。我们可以根据这个事件去做一些事情。

要注意的是，这个 storage 事件会在其它的窗口或者标签里面发生。

也就是，数据发生改变的这个窗口，不会触发 storage 事件。但是在其它的窗口可以接收到这个事件。前提是这些窗口或者标签可以访问到发生变化的 storage 数据。

#### 实例

`index.html`

```
<!doctype html>
<html lang="zh-hans">
<head>
    <meta charset="UTF-8">
    <title>Storage Event</title>
    <link rel="stylesheet" href="http://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap.min.css">
</head>
<body>
    <div class="container">
        <div class="row" style="padding: 0 25px">
            <div class="page-header">
                <h1 id="buttons">localStorage</h1>
            </div>
            <button id="set-storage" class="btn btn-primary">设置数据项目</button>
            <button id="clear-storage" class="btn btn-danger">清除数据项目</button>
        </div>
    </div>
    
</body>
    <script src="script.js"></script>    
</html>
```

`script.js`

```
// 设置数据
function setStorage() {
    localStorage.setItem('name', '好程序员');
}

// 清空数据
function clearStorage() {
    localStorage.clear();
}

// 处理 storage 事件
function storageEventHandle(event) {
    console.log(
        '数据名称：' + event.key + '\n' +
        '以前的值：' + event.oldValue + '\n' +
        '新的值：' + event.newValue + '\n' +
        '链接：' + event.url + '\n' +
        '存储：' + event.storageArea
    );
}

// 监听 设置数据项目 按钮
var setStorageBtn = document.getElementById('set-storage');
setStorageBtn.addEventListener('click', setStorage, false);

// 监听 清除数据项目 按钮
var clearStorageBtn = document.getElementById('clear-storage');
clearStorageBtn.addEventListener('click', clearStorage, false);

// 监听存储区域变化事件
window.addEventListener('storage', storageEventHandle, false);
```

### 作用域

localStorage 的作用域，也就是它的有效的应用范围，取决于文档的来源。同一来源的文档可以互相使用定义的 localStorage 数据。

这个文档的来源是根据他们的主机名，端口号，还有协议来定义的。

比如这几个例子, 都是不同的来源：

http://www.baidu.net
https://www.baidu.net
http://blog.baidu.net
http://baidu.net:8080

另外 localStorage 的作用域还跟浏览器有关，也就是你在 chrome 浏览器上设置的 localStorage 数据，在 firefox 浏览器上是访问不到的。

**实例演示**

1、不同来源

2、相同来源，不同文件

3、不同浏览器

### 数据转换

**转换成数据类型**

```
localStorage.class = 1011
typeof(localStorage.class) // string
var class = parseInt(localStorage.class)
typeof(class) // number
```

**转换成日期**

```
localStorage.lastVisitTime = (new Date()).toUTCString()
var lastVisitTime = new Date(Date.parse(localStorage.lastVisitTime))
typeof(lastVisitTime) // object
lastVisitTime.getMonth() // 4
lastVisitTime.getFullYear() // 2019
```

**转换成对象**

```
localStorage.clear()
var Class = {
	name: 'gp1011',
	size: 88
}
localStorage.classObj = JSON.stringify(Class)
var classObj = JSON.parse(localStorage.classObj)
classObj.name // gp1011
```

### 属性

**length 与 key()**

```
// 找到显示存储数据的容器
var storageData = document.getElementById('storage-data');

// 调用 显示数据 函数
displayStorageData();

// 设置数据
function setStorage() {
    localStorage.setItem('name', '好程序员')
		localStorage.setItem('size', 88)
    displayStorageData();
}

// 显示数据
function displayStorageData() {
    if (localStorage.length) {
        storageData.innerHTML = '';
        for (var i = 0; i < localStorage.length; i++) {
            var name = localStorage.key(i);
            var value = localStorage.getItem(name);
            storageData.innerHTML += '<dt>' + name + '</dt>' + '<dd>' + value + '</dd>';
        }
    }
}

// 清空数据
function clearStorage() {
    localStorage.clear();
    storageData.innerHTML = '<div class="alert alert-success">清空了 localStorage 数据！</div>';
}

// 处理 storage 事件
function storageEventHandle(event) {
    console.log(
        '数据名称：' + event.key + '\n' +
        '以前的值：' + event.oldValue + '\n' +
        '新的值：' + event.newValue + '\n' +
        '链接：' + event.url + '\n' +
        '存储：' + event.storageArea
    );
}

// 监听 设置数据项目 按钮
var setStorageBtn = document.getElementById('set-storage');
setStorageBtn.addEventListener('click', setStorage, false);

// 监听 清除数据项目 按钮
var clearStorageBtn = document.getElementById('clear-storage');
clearStorageBtn.addEventListener('click', clearStorage, false);

// 监听存储区域变化事件
window.addEventListener('storage', storageEventHandle, false);
```

### Session Storage

**案例**

`index.html`

```
<!doctype html>
<html lang="zh-hans">
<head>
    <meta charset="UTF-8">
    <title>Session Storage</title>
    <link rel="stylesheet" href="http://netdna.bootstrapcdn.com/bootstrap/3.0.0/css/bootstrap.min.css">
</head>
<body>
    <div class="container">
        <div class="row" style="padding: 0 25px">
            <div class="page-header">
                <h1 id="buttons">sessionStorage</h1>
            </div>
            <div class="row">
            <div class="col-md-6"> 
                <dl id="storage-data" class="dl-horizontal">
                    <div class='alert alert-warning'> 还没有设置存储数据！ </div>
                </dl>
            </div>
            <form id="set-form" class="col-md-6">
                <div class="form-group">
                    <label>姓名</label>
                    <input type="text" class="form-control" id="" name="name" placeholder="输入您的姓名">
                </div>
                <div class="form-group">
                    <label>性别</label>
                    <input type="text" class="form-control" id="" name="gender" placeholder="输入您的性别">
                </div>
                <button id="clear-storage" class="btn btn-danger">清除数据项目</button>
                <button type="submit" id="set-storage" class="btn btn-primary">设置数据项目</button>
            </form>
            </div>
        </div>
    </div>
    
</body>
    <script src="script.js"></script>    
</html>
```

`script.js`

```
// 找到显示存储数据的容器
var storageData = document.getElementById('storage-data');

// 调用 显示数据 函数
displayStorageData();

// 设置数据
function setStorage() {
    var setForm = document.getElementById('set-form');
    sessionStorage.setItem('name', setForm.elements['name'].value);
    sessionStorage.setItem('gender', setForm.elements['gender'].value);
    displayStorageData();
}

// 显示数据
function displayStorageData() {
    if (sessionStorage.length) {
        storageData.innerHTML = '';
        for (var i = 0; i < sessionStorage.length; i++) {
            var name = sessionStorage.key(i);
            var value = sessionStorage.getItem(name);
            storageData.innerHTML += '<dt>' + name + '</dt>' + '<dd>' + value + '</dd>';
        }
    }
}

// 清空数据
function clearStorage() {
    sessionStorage.clear();
    storageData.innerHTML = '<div class="alert alert-success">清空了 sessionStorage 数据！</div>';
}

// 处理 storage 事件
function storageEventHandle(event) {
    console.log(
        '数据名称：' + event.key + '\n' +
        '以前的值：' + event.oldValue + '\n' +
        '新的值：' + event.newValue + '\n' +
        '链接：' + event.url + '\n' +
        '存储：' + event.storageArea
    );
}

// 监听 设置数据项目 按钮
var setStorageBtn = document.getElementById('set-storage');
setStorageBtn.addEventListener('click', setStorage, false);

// 监听 清除数据项目 按钮
var clearStorageBtn = document.getElementById('clear-storage');
clearStorageBtn.addEventListener('click', clearStorage, false);

// 监听存储区域变化事件
window.addEventListener('storage', storageEventHandle, false);
```



## 应用缓存

使用 HTML5，通过创建 cache manifest 文件，可以轻松地创建 web 应用的离线版本。

### 什么是应用程序缓存

HTML5 引入了应用程序缓存，这意味着 web 应用可进行缓存，并可在没有因特网连接时进行访问。

应用程序缓存为应用带来三个优势：

- 离线浏览 - 用户可在应用离线时使用它们
- 速度 - 已缓存资源加载得更快
- 减少服务器负载 - 浏览器将只从服务器下载更新过或更改过的资源。

### HTML5 Cache Manifest 实例
```
<!DOCTYPE HTML>
<html manifest="demo.appcache">

<body>
The content of the document......
</body>

</html>
```
### Cache Manifest 基础
如需启用应用程序缓存，请在文档的 <html> 标签中包含 manifest 属性：
```
<!DOCTYPE HTML>
<html manifest="demo.appcache">
...
</html>
```
每个指定了 manifest 的页面在用户对其访问时都会被缓存。如果未指定 manifest 属性，则页面不会被缓存（除非在 manifest 文件中直接指定了该页面）。

manifest 文件的建议的文件扩展名是：".appcache"。

请注意，manifest 文件需要配置正确的 MIME-type，即 "text/cache-manifest"。**必须在 web 服务器上进行配置。**
### Manifest 文件

manifest 文件是简单的文本文件，它告知浏览器被缓存的内容（以及不缓存的内容）。

manifest 文件可分为三个部分：

- *CACHE MANIFEST* - 在此标题下列出的文件将在首次下载后进行缓存
- *NETWORK* - 在此标题下列出的文件需要与服务器的连接，且不会被缓存
- *FALLBACK* - 在此标题下列出的文件规定当页面无法访问时的回退页面（比如 404 页面）

**CACHE MANIFEST**

第一行，CACHE MANIFEST，是必需的：

```
CACHE MANIFEST
/theme.css
/logo.gif
/main.js
```

上面的 manifest 文件列出了三个资源：一个 CSS 文件，一个 GIF 图像，以及一个 JavaScript 文件。当 manifest 文件加载后，浏览器会从网站的根目录下载这三个文件。然后，无论用户何时与因特网断开连接，这些资源依然是可用的。

**NETWORK**

下面的 NETWORK 小节规定文件 "login.php" 永远不会被缓存，且离线时是不可用的：

```
NETWORK:
login.php
```

可以使用星号来指示所有其他资源/文件都需要因特网连接：

```
NETWORK:
*
```

**FALLBACK**

下面的 FALLBACK 小节规定如果无法建立因特网连接，则用 "offline.html" 替代 /html5/ 目录中的所有文件：

```
FALLBACK:
/html5/ /offline.html
```

**注释：**第一个 URI 是资源，第二个是替补。

### 更新缓存

一旦应用被缓存，它就会保持缓存直到发生下列情况：

- 用户清空浏览器缓存
- manifest 文件被修改（参阅下面的提示）
- 由程序来更新应用缓存

**实例 - 完整的 Manifest 文件**

```
CACHE MANIFEST
# v1.1

CACHE:

../css/bootstrap.min.css
../js/jquery-2.0.3.min.js
../js/bootstrap.min.js
script.js

NETWORK:

*

FALLBACK:

../images/ ../images/offline.png
/appcache-files/01-01/ /appcache-files/01-01/offline.html
```

**重要的提示：**

以 "#" 开头的是注释行，但也可满足其他用途。应用的缓存会在其 manifest 文件更改时被更新。如果您编辑了一幅图片，或者修改了一个 JavaScript 函数，这些改变都不会被重新缓存。更新注释行中的日期和版本号是一种使浏览器重新缓存文件的办法。

浏览器对缓存数据的容量限制可能不太一样（某些浏览器设置的限制是每个站点 5MB）。

### 案例

**1、目录结构**

![image-20190526065454780](/Users/Felix/Library/Application Support/typora-user-images/image-20190526065454780.png)

**2、01-01**

`index.html`

```
<!doctype html>
<html lang="zh-hans" manifest="offline.appcache">

<head>
    <meta charset="UTF-8">
    <title>Application Cache</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
    <style>
        img{
            width:100%;
            margin-bottom: 18px;
            background:#eee;
        }
        #update{
            clear:both;
        }
        #gallery, .page-header{
            padding-left: 39px;
            padding-right: 39px;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="page-header">
                <h1 id="title">Application Cache</h1>
                <div>
                    <a href="#" data-toggle="popover" data-content="摄影作品" data-original-title="标题">这是应用缓存的演示</a>
                </div>
            </div>
            <div class="row" id="gallery">
                <div class="col-md-6">
                    <a href="gallery-1.html">
                        <img class="" src="../images/06.jpg" alt="图像 1">
                    </a>
                </div>
                <div class="col-md-6">
                    <img class="" src="../images/03.jpg" alt="图像 2">
                </div>
            </div>
            <div id="message"></div>
        </div>
    </div>
</body>
<script src="../js/jquery-2.0.3.min.js"></script>
<script src="../js/bootstrap.min.js"></script>
<script src="script.js"></script>

</html>
```

`offline.appcache`

```
CACHE MANIFEST
# v1.1

CACHE:

../css/bootstrap.min.css
../js/jquery-2.0.3.min.js
../js/bootstrap.min.js
script.js

NETWORK:

*

FALLBACK:

../images/ ../images/offline.png
/appcache-files/01-01/ /appcache-files/01-01/offline.html
```

`offline.html`

```
<!doctype html>
<html lang="zh-hans" manifest="offline.appcache">
<head>
    <meta charset="UTF-8">
    <title>离线</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>
<body>
    <div class="container">
        <div class="alert alert-warning" style="text-align:center;width:500px;margin: 50px auto">现在是离线状态，没法儿打开您请求的页面。</div>
    </div>
</body>
</html>
```

**3、02-02 **

`index.html`

```
<!doctype html>
<html lang="zh-hans" manifest="offline.appcache">

<head>
    <meta charset="UTF-8">
    <title>updateready</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
    <style>
        img{
            width:100%;
            margin-bottom: 18px;
            background:#eee;
        }
        #update{
            clear:both;
        }
        #gallery, .page-header{
            padding-left: 39px;
            padding-right: 39px;
        }
        .alert{
            margin-left: 39px;
            margin-right: 39px;
        }
    </style>
</head>

<body>
    <div class="container">
        <div class="row">
            <div class="page-header">
                <h1 id="title">updateready</h1>
            </div>
            <div class="row" id="gallery">
                <div id="update"></div>
                <div class="col-md-6">
                    <a href="gallery-1.html">
                        <img class="" src="../images/06.jpg" alt="图像 1">
                    </a>
                </div>
                <div class="col-md-6">
                    <img class="" src="../images/03.jpg" alt="图像 2">
                </div>
            </div>
            <div id="message"></div>
        </div>
    </div>
</body>
<script src="../js/jquery-2.0.3.min.js"></script>
<script src="../js/bootstrap.min.js"></script>
<script src="script.js"></script>

</html>
```

`offline.html`

```
<!doctype html>
<html lang="zh-hans" manifest="offline.appcache">
<head>
    <meta charset="UTF-8">
    <title>离线</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
</head>
<body>
    <div class="container">
        <div class="alert alert-warning" style="text-align:center;width:500px;margin: 50px auto">现在是离线状态，没法儿打开您请求的页面。</div>
    </div>
</body>
</html>
```

`offline.appcache`

```
CACHE MANIFEST
# v1.121

CACHE:

../css/bootstrap.min.css
../js/jquery-2.0.3.min.js
../js/bootstrap.min.js
script.js

NETWORK:

*

FALLBACK:

../images/ ../images/offline.png
/appcache-files/02-02/ /appcache-files/02-02/offline.html
```

**03-01**

`index.html`

```
<!doctype html>
<html lang="zh-hans" >
<head>
    <meta charset="UTF-8">
    <title>offline app</title>
    <link rel="stylesheet" href="../css/bootstrap.min.css">
    <style>
       .success {
    		background-color: #5cb85c;
    	}
    </style>
</head>
<body>
    <div class="container">
        <div class="row" style="padding: 0 25px">
            <div class="page-header">
                <h1 id="buttons">offline app <span id="online-status" class="badge success">在线</span></h1>
            </div>
            <div class="row">
            <div class="col-md-6"> 
                <dl id="storage-data" class="dl-horizontal">
                    <div class='alert alert-warning'> 还没有设置存储数据！ </div>
                </dl>
            </div>
            <form id="set-form" class="col-md-6">
                <div class="form-group">
                    <label>姓名</label>
                    <input type="text" class="form-control" id="" name="name" placeholder="输入您的姓名">
                </div>
                <div class="form-group">
                    <label>性别</label>
                    <input type="text" class="form-control" id="" name="gender" placeholder="输入您的性别">
                </div>
                <button id="clear-storage" class="btn btn-danger">清除数据项目</button>
                <button type="submit" id="set-storage" class="btn btn-primary">设置数据项目</button>
            </form>
            </div>
        </div>
    </div>
    
</body>
    <script src="script.js"></script>    
</html>
```

`offline.appcache`

```
CACHE MANIFEST

# v1

CACHE:
../css/bootstrap.min.css
script.js
```

`script.js`

```
function onlineStatus() {
    var status = document.getElementById('online-status');
    if (navigator.onLine) {
        status.innerHTML = '在线';
        status.className = 'badge success';
    } else {
        status.innerHTML = '离线';
        status.className = 'badge';
    }
}

onlineStatus();

window.addEventListener('online', onlineStatus, false);
window.addEventListener('offline', onlineStatus, false);

// 找到显示存储数据的容器
var storageData = document.getElementById('storage-data');

// 调用 显示数据 函数
displayStorageData();

// 设置数据
function setStorage(event) {
    var setForm = document.getElementById('set-form');
    sessionStorage.setItem('name', setForm.elements['name'].value);
    sessionStorage.setItem('gender', setForm.elements['gender'].value);
    displayStorageData();
    event.preventDefault();
}

// 显示数据
function displayStorageData() {
    if (sessionStorage.length) {
        storageData.innerHTML = '';
        for (var i = 0; i < sessionStorage.length; i++) {
            var name = sessionStorage.key(i);
            var value = sessionStorage.getItem(name);
            storageData.innerHTML += '<dt>' + name + '</dt>' + '<dd>' + value + '</dd>';
        }
    }
}

// 清空数据
function clearStorage(event) {
    sessionStorage.clear();
    storageData.innerHTML = '<div class="alert alert-success">清空了 sessionStorage 数据！</div>';
    event.preventDefault();
}

// 处理 storage 事件
function storageEventHandle(event) {
    console.log(
        '数据名称：' + event.key + '\n' +
        '以前的值：' + event.oldValue + '\n' +
        '新的值：' + event.newValue + '\n' +
        '链接：' + event.url + '\n' +
        '存储：' + event.storageArea
    );
}

// 监听 设置数据项目 按钮
var setStorageBtn = document.getElementById('set-storage');
setStorageBtn.addEventListener('click', setStorage, false);

// 监听 清除数据项目 按钮
var clearStorageBtn = document.getElementById('clear-storage');
clearStorageBtn.addEventListener('click', clearStorage, false);

// 监听存储区域变化事件
window.addEventListener('storage', storageEventHandle, false);
```

### 清理 appcache

```
chrome://appcache-internals/
```

 

## WebSQL

## 文件API
## 地理定位
### 定义

HTML5 Geolocation（地理定位）用于定位用户的位置。

HTML5 Geolocation API 用于获得用户的地理位置。

鉴于该特性可能侵犯用户的隐私，除非用户同意，否则用户位置信息是不可用的。

### 使用地理定位

请使用 getCurrentPosition() 方法来获得用户的位置。

```
<script>
var x = document.getElementById("demo");
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition, showError);
  } else {
    x.innerHTML="Geolocation is not supported by this browser.";
  }
}

function showPosition(position) {
  x.innerHTML="Latitude: " + position.coords.latitude +
  "<br />Longitude: " + position.coords.longitude;
}

function showError(error) {
  switch (error.code) {
    case error.PERMISSION_DENIED:
      x.innerHTML = "User denied the request for Geolocation."
      break;
    case error.POSITION_UNAVAILABLE:
      x.innerHTML = "Location information is unavailable."
      break;
    case error.TIMEOUT:
      x.innerHTML = "The request to get user location timed out."
      break;
    case error.UNKNOWN_ERROR:
      x.innerHTML = "An unknown error occurred."
      break;
  }
}
</script>
```



## 拖放

拖放（Drag 和 drop）是 HTML5 标准的组成部分。

拖放是一种常见的特性，即抓取对象以后拖到另一个位置。

在 HTML5 中，拖放是标准的一部分，任何元素都能够拖放。

```
<!DOCTYPE HTML>
<html>

<head>
  <script type="text/javascript">
    function allowDrop(ev) {
      ev.preventDefault();
    }

    function drag(ev) {
      ev.dataTransfer.setData("Text", ev.target.id);
    }

    function drop(ev) {
      ev.preventDefault();
      var data = ev.dataTransfer.getData("Text");
      ev.target.appendChild(document.getElementById(data));
    }
  </script>
</head>

<body>

  <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)"></div>
  <img id="drag1" src="img_logo.gif" draggable="true" ondragstart="drag(event)" width="336" height="69" />

</body>

</html>
```

### 设置元素可拖放

首先，为了使元素可拖动，把 draggable 属性设置为 true ：

```
<img draggable="true" />
```

### 拖动什么 - ondragstart 和 setData()

然后，规定当元素被拖动时，会发生什么。

在上面的例子中，ondragstart 属性调用了一个函数，drag(*event*)，它规定了被拖动的数据。

dataTransfer.setData() 方法设置被拖数据的数据类型和值：

```
function drag(ev) {
  ev.dataTransfer.setData("Text",ev.target.id);
}
```

在这个例子中，数据类型是 "Text"，值是可拖动元素的 id ("drag1")。

### 放到何处 - ondragover

ondragover 事件规定在何处放置被拖动的数据。

默认地，无法将数据/元素放置到其他元素中。如果需要设置允许放置，我们必须阻止对元素的默认处理方式。

这要通过调用 ondragover 事件的 *event*.preventDefault() 方法：

```
event.preventDefault()
```

### 进行放置 - ondrop

当放置被拖数据时，会发生 drop 事件。

在上面的例子中，ondrop 属性调用了一个函数，drop(*event*)：

```
function drop(ev) {
  ev.preventDefault(); //调用 preventDefault() 来避免浏览器对数据的默认处理（drop 事件的默认行为是以链接形式打开）
  var data = ev.dataTransfer.getData("Text"); // 通过 dataTransfer.getData("Text") 方法获得被拖的数据。该方法将返回在 setData() 方法中设置为相同类型的任何数据。被拖数据是被拖元素的 id ("drag1")
  ev.target.appendChild(document.getElementById(data)); // 把被拖元素追加到放置元素（目标元素）中
}
```

### 案例

```
<!DOCTYPE HTML>
<html>

<head>
  <style type="text/css">
    #div1,
    #div2 {
      float: left;
      width: 198px;
      height: 66px;
      margin: 10px;
      padding: 10px;
      border: 1px solid #aaaaaa;
    }
  </style>
  <script type="text/javascript">
    function allowDrop(ev) {
      ev.preventDefault();
    }

    function drag(ev) {
      ev.dataTransfer.setData("Text", ev.target.id);
    }

    function drop(ev) {
      ev.preventDefault();
      var data = ev.dataTransfer.getData("Text");
      ev.target.appendChild(document.getElementById(data));
    }
  </script>
</head>

<body>

  <div id="div1" ondrop="drop(event)" ondragover="allowDrop(event)">
    <img src="http://placehold.it/100x100" draggable="true" ondragstart="drag(event)" id="drag1" />
  </div>
  <div id="div2" ondrop="drop(event)" ondragover="allowDrop(event)"></div>

</body>

</html>
```



## 全屏
使用HTML5提供的JavaScript Api可以实现主流浏览器的全屏和退出全屏操作。

```
<!DOCTYPE html>
<html>
<head>
    <meta charset="utf-8">
    <title>全屏切换</title>
    <script type="text/javascript">
    //进入全屏
    function enterFullScreen() {
        var de = document.documentElement;
        if (de.requestFullscreen) {
            de.requestFullscreen();
        } else if (de.mozRequestFullScreen) {
            de.mozRequestFullScreen();
        } else if (de.webkitRequestFullScreen) {
            de.webkitRequestFullScreen();
        }
    }
    //退出全屏
    function exitFullScreen() {
        var de = document;
        if (de.exitFullscreen) {
            de.exitFullscreen();
        } else if (de.mozCancelFullScreen) {
            de.mozCancelFullScreen();
        } else if (de.webkitCancelFullScreen) {
            de.webkitCancelFullScreen();
        }
    }
    </script>
</head>
<body>
    <div>
        <a href="javascript:;" onclick="enterFullScreen()">进入全屏</a>
        &nbsp;
        <a href="javascript:;" onclick="exitFullScreen()">退出全屏</a>
    </div>
</body>
</html>
```



## 网络状态

### 网络状态属性

window.navigator.onLine 返回浏览器的网络状态。联网状态时返回true，断网状态时返回false。
 注意：各浏览器对该属性的实现有些不同。

 在Chrome和Safari中，如果浏览器连接不上局域网 (LAN)或者路由器，就是断网状态；否则就是联网状态。所以当该属性值为false的时候，你可以说浏览器不能正常联网，但如果该属性值为true的时候，并不意味着浏览器一定能连接上互联网。还有其他一些可能引起误判的原因，比如你的电脑安装了虚拟化软件，可能会有一个虚拟网卡，这时它总是会显示正常联网。

 在Firefox和Internet Explorer中，如果浏览器处于"脱机工作"状态，则返回 false，其他情况都返回true。

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>network status</title>
</head>
<body>
    <script type="text/javascript">
    // 获取当前网络状态
    var state = window.navigator.onLine;
    if (state) {
        alert("联网状态");
    }
    else {
        alert("断网状态");
    }
    </script>
</body>
</html>
```

### 网络状态事件

+ 联网时触发
```
// 不推荐，有兼容性问题
window.ononload = function() {}
或
// 推荐
window.addEventListener('online',  function() {});
```

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>online event</title>
</head>
<body>
    <script type="text/javascript">
    window.addEventListener('online',  function() {
        alert("在线");
    });
    </script>
</body>
</html>
```

+ 断网时触发
```
// 不推荐，有兼容性问题
window.onoffline = function() {}
或
// 推荐
window.addEventListener('offline',  function() {});
```

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>offline event</title>
</head>
<body>
    <script type="text/javascript">
    window.addEventListener('offline',  function() {
        alert("在掉线");
    });
    </script>
</body>
</html>
```



## WebWorker

### 什么是 Web Worker？

当在 HTML 页面中执行脚本时，页面的状态是不可响应的，直到脚本已完成。

web worker 是运行在后台的 JavaScript，独立于其他脚本，不会影响页面的性能。您可以继续做任何愿意做的事情：点击、选取内容等等，而此时 web worker 在后台运行。

### 检测 Web Worker 支持

在创建 web worker 之前，请检测用户的浏览器是否支持它：

```
if (typeof (Worker) !== "undefined") {
  // Yes! Web worker support!
  // Some code.....
} else {
  // Sorry! No Web Worker support..
}
```

### 创建 web worker 文件

现在，让我们在一个外部 JavaScript 中创建我们的 web worker。

在这里，我们创建了计数脚本。该脚本存储于 "demo_workers.js" 文件中：

```
var i = 0;

function timedCount() {
  i = i + 1;
  postMessage(i);
  setTimeout("timedCount()", 500);
}

timedCount();
```

以上代码中重要的部分是 *postMessage()* 方法 - 它用于向 HTML 页面传回一段消息。

**注释：**web worker 通常不用于如此简单的脚本，而是用于更耗费 CPU 资源的任务。

### 创建 Web Worker 对象

我们已经有了 web worker 文件，现在我们需要从 HTML 页面调用它。

下面的代码检测是否存在 worker，如果不存在，- 它会创建一个新的 web worker 对象，然后运行 "demo_workers.js" 中的代码：

```
if (typeof (w) == "undefined") {
  w = new Worker("demo_workers.js");
}

timedCount();
```

然后我们就可以从 web worker 发生和接收消息了。

向 web worker 添加一个 "onmessage" 事件监听器：

```
w.onmessage = function (event) {
  document.getElementById("result").innerHTML = event.data;
};
```

当 web worker 传递消息时，会执行事件监听器中的代码。event.data 中存有来自 event.data 的数据。

### 终止 Web Worker

当我们创建 web worker 对象后，它会继续监听消息（即使在外部脚本完成之后）直到其被终止为止。

如需终止 web worker，并释放浏览器/计算机资源，请使用 terminate() 方法：

```
w.terminate();
```



## history

## WebSocket



# CSS3

## CSS3选择器
### 基本选择器
**通配选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>通配选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      background: red;
    }
    ul li {
      width: 80px;
      height: 80px;
      margin-left: 10px;
      display: inline-block;
      border: 1px solid #000;
    }
    ul * {
      background: yellow;
    }
  </style>
</head>
<body>
  <div>
    <ul>
      <li>1</li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
      <li>8</li>
      <li>9</li>
      <li>10</li>
    </ul>
  </div>
</body>
</html>
```
**元素选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>元素选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      background: red;
    }
    ul li {
      width: 80px;
      height: 80px;
      margin-left: 10px;
      display: inline-block;
      border: 1px solid #000;
    }
    ul * {
      background: yellow;
    }
    span {
      background: blue;
    }
  </style>
</head>
<body>
  <div>
    <ul>
      <li>
        <span>first</span>
      </li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
      <li>8</li>
      <li>9</li>
      <li>10</li>
    </ul>
  </div>
</body>
</html>
```
**ID选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>ID选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      background: red;
    }
    ul li {
      width: 80px;
      height: 80px;
      margin-left: 10px;
      display: inline-block;
      border: 1px solid #000;
    }
    ul * {
      background: yellow;
    }
    span {
      background: blue;
    }

    #last {
      background: purple;
    }
  </style>
</head>
<body>
  <div>
    <ul>
      <li>
        <span>first</span>
      </li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
      <li>8</li>
      <li>9</li>
      <li id="last">10</li>
    </ul>
  </div>
</body>
</html>
```
**类选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>类选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      background: red;
    }
    ul li {
      width: 80px;
      height: 80px;
      margin-left: 10px;
      display: inline-block;
      border: 1px solid #000;
    }
    ul * {
      background: yellow;
    }
    span {
      background: blue;
    }

    #last {
      background: purple;
    }

    .child {
      background: gray;
    }
  </style>
</head>
<body>
  <div>
    <ul>
      <li>
        <span>first</span>
      </li>
      <li>2</li>
      <li class="child">3</li>
      <li class="child">4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
      <li>8</li>
      <li>9</li>
      <li id="last">10</li>
    </ul>
  </div>
</body>
</html>
```
**群组选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>群组选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      background: #444;
    }
    ul li {
      width: 80px;
      height: 80px;
      margin-left: 10px;
      display: inline-block;
      border: 1px solid #000;
    }
    ul * {
      background: yellow;
    }
    span {
      background: blue;
    }

    #last {
      background: purple;
    }

    .child {
      background: gray;
    }

    .item1, #item2 {
      background: tomato;
    }
  </style>
</head>
<body>
  <div>
    <ul>
      <li>
        <span>first</span>
      </li>
      <li class="item1">2</li>
      <li class="child">3</li>
      <li class="child">4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
      <li>8</li>
      <li id="item2">9</li>
      <li id="last">10</li>
    </ul>
  </div>
</body>
</html>
```
### 层次选择器

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>层次选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    body {
      width: 300px;
      margin: 0 auto;
    }
    div {
      margin: 5px;
      padding: 5px;
      border: 1px solid #ccc;
    }

    /* 后代选择器 */
    div div {
      background: orange;
    }

    /* 子选择器 */
    body > div {
      background: green;
    }

    /* 相邻兄弟选择器 */
    .active + div {
      background: #ccc;
    }

    /* 通用兄弟选择器 */
    .active ~ div {
      background: red;
    }
  </style>
</head>
<body>
  <div class="active">1</div>
  <div>2</div>
  <div>3</div>
  <div>4
    <div>5</div>
    <div>6</div>
  </div>
  <div>7
    <div>8
      <div>9
        <div>10</div>
      </div>
    </div>
  </div>
</body>
</html>
```
### 伪类选择器
**动态伪类选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>动态伪类选择器</title>
  <style>
    div {
      text-align: center;
    }
    .btn {
      background: #0074cc;
      border: 1px solid #ccc;
      color: #fff;
      font-size: 20px;
      padding: 14px 24px;
      text-align: center;
      text-decoration: none;
      vertical-align: middle;
    }
    .btn:hover {
      background: #0055cc;
    }
    .btn:active {
      background: #004ab3;
    }
    .btn:focus {
      outline: thin dotted #333;
    }
  </style>
</head>
<body>
  <div>
    <a href="#" class="btn">动态伪类选择器按钮</a>
  </div>
</body>
</html>
```
**目标伪类选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>目标伪类选择器</title>
  <style>
    .menu {
      color: #424242;
      margin: 0 auto;
      padding: 10px;
      width: 500px;
    }
    .menu h2 {
      margin: 5px 0;
      padding: 0;
      position: relative;
    }
    .menu h2 a {
      background: #8f8f8f;
      border-radius: 5px;
      display: block;
      font-size: 13px;
      color: #424242;
      margin: 0;
      padding: 10px;
      text-decoration: none;
    }

    .menu :target h2 a,
    .menu h2 a:focus,
    .menu h2 a:hover,
    .menu h2 a:active {
      background: #2288dd;
      color: #fff;
    }

    .menu p {
      margin: 0;
      padding: 0;
      overflow: hidden;
      padding: 0 10px;
      height: 0;
    }

    .menu :target p {
      overflow: auto;
      height: 50px;
    }
  </style>
</head>
<body>
  <div class="menu">
    <div class="menuSection" id="basic">
      <h2><a href="#basic">前端开发基础</a></h2>
      <p>HTML + CSS + JavaScript</p>
    </div>
    <div class="menuSection" id="tools">
      <h2><a href="#tools">前端工程化工具</a></h2>
      <p>Gulp + Webpack</p>
    </div>
    <div class="menuSection" id="framework">
      <h2><a href="#framework">前端开发框架</a></h2>
      <p>Vue + React + Angular</p>
    </div>
  </div>
</body>
</html>
```
**语言伪类选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>语言伪类选择器</title>
  <style>
    :lang(en) {
      font-family: Arial, Helvetica, sans-serif;
      font-size: 32px;
      quotes: '"' '"';
    }
    :lang(zh-cn) {
      font-family: 宋体;
      font-size: 16px;
      quotes: '“' '”';
    }
  </style>
</head>
<body>
  <p>
    Language pseudo-class selector
  </p>
  <p lang="en"><q>Quote in English</q></p>
  <p lang="zh-cn"><q>中文的引号</q></p>
</body>
</html>
```
**UI元素状态选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>UI元素状态选择器</title>
  <style>
    input[type=radio] {
      margin-right: 10px;
      cursor: pointer;
      font-size: 14px;
      width: 12px;
      height: 12px;
      position: relative;
    }

    input[type=radio]:after {
      position: absolute;
      width: 20px;
      height: 20px;
      content: " ";
      background: #2288dd;
      color: #fff;
      top: -5px;
      border-radius: 50%;
    }

    input[type=radio]:checked:before {
      content: '✔';
      position: absolute;
      top: -3px;
      left: 5px;
      color: #fff;
      font-weight: 100;
      z-index: 1;
    }

    input[type=checkbox] {
      margin-right: 10px;
      position: relative;
      font-size: 14px;
    }

    input[type=checkbox]:enabled:after,
    input[type=checkbox]:disabled:after {
      position: absolute;
      width: 20px;
      height: 20px;
      content: ' ';
      background: #2288dd;
      color: #fff;
      top: -5px;
      left: -5px;
      border-radius: 20%;
    }

    input[type=checkbox]:disabled:after {
      background: #ccc;
    }

    input[type=checkbox]:checked:before {
      content: '✔';
      position: absolute;
      top: -3px;
      color: #fff;
      font-weight: 100;
      z-index: 1;
    }
  </style>
</head>
<body>
  <form action="">
    <label for="">
      性别：
      男：<input name="gender" checked type="radio" />
      女：<input name="gender" type="radio" />
    </label>
    <br />
    <label for="">
      年龄：
      0-17岁 <input disabled type="checkbox" />
      18-35岁 <input enabled checked type="checkbox" />
      35岁及以上 <input type="checkbox" />
    </label>
  </form>
</body>
</html>
```
**结构伪类选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>结构伪类选择器</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    ul {
      margin: 50px auto;
      width: 400px;
      list-style: none outside none;
    }
    ul li, ul div {
      display: inline-block;
      margin: 5px;
      padding: 5px;
      width: 50px;
      height: 50px;
      font: bold 30px/50px arial;
      background: #000;
      color: #fff;
      border-radius: 50%;
      text-align: center;
    }

    /* :first-child */
    /* ul>li:first-child {
      background: green;
    } */

    /* :last-child */
    /* ul>li:last-child {
      background: blue;
    } */

    /* :nth-child */
    /* ul>li:nth-child(3) {
      background: yellow;
    } */
    /* ul>li:nth-child(n) {
      background: blue;
    } */
    /* ul>li:nth-child(2n) {
      background: blue;
    } */
    /* ul>li:nth-child(2n+1) {
      background: blue;
    } */
    /* ul>li:nth-child(even) {
      background: blue;
    } */
    /* ul>li:nth-child(odd) {
      background: blue;
    } */
    /* ul>li:nth-child(2n-1) {
      background: blue;
    } */
    /* ul>li:nth-child(n+5) {
      background: blue;
    } */
    /* ul>li:nth-child(-n+5) {
      background: blue;
    } */
    /* ul>li:nth-child(4n+1) {
      background: blue;
    } */
    /* ul>li:nth-child(21) {
      background: blue;
    } */

    /* :nth-of-type */
    /* ul>div:nth-of-type(1) {
      background: blue;
    } */

    /* :nth-last-of-type() */
    /* ul>div:nth-last-of-type(1) {
      background: blue;
    } */

    /* :first-of-type */
    /* ul>div:first-of-type {
      background: blue;
    } */

    /* :last-of-type */
    /* ul>div:last-of-type {
      background: blue;
    } */

    /* :only-child */
    /* ul>div:only-child {
      background: blue;
    } */

    /* :only-of-type */
    /* ul>div:only-of-type {
      background: blue;
    } */

    /* :empty */
    ul>div:nth-of-type(2):empty {
      background: blue;
      border-radius: 0%;
    }
  </style>
</head>
<body>
  <ul>
    <li>1</li>
    <li>2</li>
    <li>3</li>
    <li>4</li>
    <li>5</li>
    <li>6</li>
    <li>7</li>
    <li>8</li>
    <li>9</li>
    <li>10</li>
    <li>11</li>
    <li>12</li>
    <li>13</li>
    <li>14</li>
    <div>21</div>
    <li>15</li>
    <li>16</li>
    <li>17</li>
    <li>18</li>
    <li>19</li>
    <li>20</li>
    <div> </div>
  </ul>
</body>
</html>
```
**否定选择器**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>否定选择器</title>
  <style>
    /* input {
      border: 1px solid #2277cc;
      width: 150px;
    } */
    input:not([type=radio]) {
      border: 1px solid #2277cc;
      width: 150px;
    }
  </style>
</head>
<body>
  <form action="">
    姓名：<input type="text" />
    邮编：<input type="text" />
    性别：<input type="radio" /> 男 <input type="radio" /> 女
  </form>
</body>
</html>
```

### 伪元素

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>伪元素</title>
  <style>
    p {
      width: 200px;
      margin: 0 auto;
    }

    p::first-letter {
      color: #903;
      float: left;
      padding: 4px 8px 0 3px;
      font: 75px/60px Georgia;
    }

    p::first-line {
      font: italic 16px/18px Georgia;
      color: #903;
    }

    p::before {
      content: 'React';
    }

    p::after {
      content: '→'
    }

    p::selection {
      background: red;
      color: #fff;
    }
  </style>
</head>
<body>
  <p>可以轻松创建交互式用户界面。为应用程序中的每个状态设计简单的视图，当数据更改时，React 将高效地更新和正确的渲染组件。</p>
</body>
</html>
```

### 属性选择器

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>属性选择器</title>
  <style>
    ul {
      width: 300px;
      margin: 0 auto;
      border: 1px solid #ccc;
      padding: 10px;
      overflow: hidden;
      margin: 20px auto;
      list-style: none;
    }

    ul li {
      float: left;
      height: 50px;
      width: 50px;
      border-radius: 10px;
      text-align: center;
      background: #aac;
      color: blue;
      font: bold 20px/50px Arial;
      margin: 5px;
    }

    /* li[id] {
      background: yellow;
    } */

    /* li[id=first] {
      background: yellow;
    } */

    /* li[class=item] {
      background: yellow;
    } */

    /* li[class='item item6'] {
      background: yellow;
    } */

    /* li[lang|=zh] {
      background: yellow;
    } */

    /* li[class~=item] {
      background: yellow;
    } */

    /* li[class*=item] {
      background: yellow;
    } */

    /* li[class^=item] {
      background: yellow;
    } */

    li[class$=item] {
      background: yellow;
    }
  </style>
</head>
<body>
  <ul>
    <li id="first" class="item first">1</li>
    <li>2</li>
    <li lang="zh-cn">3</li>
    <li class="item">4</li>
    <li>5</li>
    <li class="item item6">6</li>
    <li>7</li>
    <li class="eightitem">8</li>
    <li>9</li>
    <li id="last">10</li>
  </ul>
</body>
</html>
```
## CSS3盒模型
### box-sizing

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>css3 box-sizing</title>
  <style>
    .content-box {
      width: 200px;
      padding: 30px;
      border: solid blue 20px;
      box-sizing: content-box;
    }
    .border-box {
      width: 200px;
      padding: 30px;
      border: solid blue 20px;
      box-sizing: border-box;
    }
  </style>
</head>
<body>
  <div class="content-box">
    Vue是一套用于构建用户界面的渐进式框架。与其它大型框架不同的是，Vue 被设计为可以自底向上逐层应用。Vue 的核心库只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合。
  </div>
  <div class="border-box">
    Vue是一套用于构建用户界面的渐进式框架。与其它大型框架不同的是，Vue 被设计为可以自底向上逐层应用。Vue 的核心库只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合。
  </div>
</body>
</html>
```

### CSS3 溢出隐藏属性

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>CSS3 溢出隐藏属性</title>
  <style>
    div {
      width: 150px;
      height: 100px;
      overflow-y: no-display;
    }
  </style>
</head>
<body>
  <div>
      Vue是一套用于构建用户界面的渐进式框架。与其它大型框架不同的是，Vue 被设计为可以自底向上逐层应用。Vue 的核心库只关注视图层，不仅易于上手，还便于与第三方库或既有项目整合。
  </div>
</body>
</html>
```

### resize

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>resize</title>
  <style>
    textarea {
      resize: none;
    }
  </style>
</head>
<body>
  <form action="">
    <textarea name="" id="" cols="30" rows="10"></textarea>
  </form>
</body>
</html>
```

### outline

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>outline</title>
  <style>
    input {
      outline-width: 3px;
      outline-color: red;
      outline-style: dotted;
      outline-offset: -3px;
    }
  </style>
</head>
<body>
  <form action="">
    <input type="text" />
  </form>
</body>
</html>
```



## CSS3弹性盒布局模型

### flex 容器

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>flexbox-容器</title>
  <style>
    body {
      margin: 0;
      padding: 0;
    }
    .container {
      height: 500px;
      background: purple;
      padding: 10px;
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      /* align-items: flex-start; */
      align-content: space-around;
    }
    .item {
      background: orange;
      color: purple;
      padding: 30px;
      display: block;
      text-align: center;
      border-left: 1px solid purple;
      border-bottom: 1px solid purple;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="item item-1"><span>1</span></div>
    <div class="item item-2"><span>2</span></div>
    <div class="item item-3"><span>3</span></div>
    <div class="item item-4"><span>4</span></div>
    <div class="item item-5"><span>5</span></div>
    <div class="item item-6"><span>6</span></div>
    <div class="item item-7"><span>7</span></div>
    <div class="item item-8"><span>8</span></div>
    <div class="item item-9"><span>9</span></div>
    <div class="item item-10"><span>10</span></div>
    <div class="item item-11"><span>11</span></div>
    <div class="item item-12"><span>12</span></div>
  </div>
</body>
</html>
```

### flex 项目

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>flexbox-项目属性</title>
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      margin: 0;
      padding: 0;
    }
    .container {
      width: 450px;
      height: 500px;
      background: purple;
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      justify-content: space-around;
    }
    .item {
      background: orange;
      color: purple;
      padding: 30px;
      display: block;
      text-align: center;
      border-left: 1px solid purple;
      border-bottom: 1px solid purple;
    }
    .item-1, .item-5 {
      align-self: flex-end;
    }
    .item-2, .item-4 {
      align-self: center;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="item item-1"><span>1</span></div>
    <div class="item item-2"><span>2</span></div>
    <div class="item item-3"><span>3</span></div>
    <div class="item item-4"><span>4</span></div>
    <div class="item item-5"><span>5</span></div>
  </div>
</body>
</html>
```
## CSS3变换
### 2D 变换
**translate**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>translate</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      width: 150px;
      height: 150px;
      background: yellow;
      transform: translate(50px, 100px);
      -ms-transform: translate(50px, 100px);		/* IE 9 */
      -webkit-transform: translate(50px, 100px);	/* Safari and Chrome */
      -o-transform: translate(50px, 100px);		/* Opera */
      -moz-transform: translate(50px, 100px);		/* Firefox */

      /* transform: translateX(50px) translateY(100px); */
    }
  </style>
</head>
<body>
  <div></div>
</body>
</html>
```
**rotate**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>rotate</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      width: 150px;
      height: 150px;
      background: yellow;
      transform: rotate(30deg);
      -ms-transform: rotate(30deg);		/* IE 9 */
      -webkit-transform: rotate(30deg);	/* Safari and Chrome */
      -o-transform: rotate(30deg);		/* Opera */
      -moz-transform: rotate(30deg);		/* Firefox */
      
      transform-origin: 0 0;
    }
  </style>
</head>
<body>
  <div></div>
</body>
</html>
```
**scale**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>scale</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      width: 150px;
      height: 150px;
      background: yellow;
      transform: scale(2,4);
      -ms-transform: scale(2,4);	/* IE 9 */
      -webkit-transform: scale(2,4);	/* Safari 和 Chrome */
      -o-transform: scale(2,4);	/* Opera */
      -moz-transform: scale(2,4);	/* Firefox */
      /* transform-origin: 0 0; */
    }
  </style>
</head>
<body>
  <div></div>
</body>
</html>
```
**skew**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>skew</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      width: 150px;
      height: 150px;
      background: yellow;
      transform: skew(30deg,20deg);
      -ms-transform: skew(30deg,20deg);	/* IE 9 */
      -webkit-transform: skew(30deg,20deg);	/* Safari and Chrome */
      -o-transform: skew(30deg,20deg);	/* Opera */
      -moz-transform: skew(30deg,20deg);	/* Firefox */
      transform-origin: 0 0;
    }
  </style>
</head>
<body>
  <div></div>
</body>
</html>
```
**matrix**
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>matrix</title>
  <style>
    * {
      margin: 0;
      padding: 0;
    }
    div {
      width: 150px;
      height: 150px;
      background: yellow;
      transform: matrix(1, 0, 0, 1, 100, 100);
      /* transform: matrix(2, 0, 0, 2, 0, 0);
      transform: matrix(0.866, 0.5, -0.5, 0.866, 0, 0);
      transform: matrix(1, 0.5, 0.5, 1, 0, 0); */
      transform-origin: 0 0;
    }

    /* transform matrix
      a c e   x
      b d f   y
      0 0 1   1

      平移：
      1 0 x
      0 1 y
      0 0 1

      缩放：
      x 0 0
      0 y 0
      0 0 1

      旋转：
      cos(x) -sin(x) 0
      sin(x) cos(x)  0
      0      0       1

      变形：
      1      tan(y) 0
      tan(x) 1      0
      0      0      1 
    */
  </style>
</head>
<body>
  <div></div>
</body>
</html>
```

### 3D 变换

**卡片翻转**

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>card flip</title>
  <style>
    body{
      perspective: 800px;
      transform-style: preserve-3d;
    }
    #box{
      width: 300px;
      height: 300px;
      margin: 0 auto;
      transform-style: preserve-3d;
      position: relative; /*相对body定位*/
      transition: 2s; /*运动时间*/
    }
    #box:hover{
      transform:rotateY(180deg); /*当鼠标移动到上面时让他旋转180°*/
    }
    #box .bian{
      width: 300px;
      height: 300px;
      text-align: center;
      line-height: 300px;
      font-size: 100px;
      position: absolute; /*.mian相对与#box绝对定位*/
    }
    #box .bian img {
      width: 100%;
      height: 100%;
    }
    .zhi1{
      background-color: red;
      transform: rotateY(180deg);
    }
    .zhi2{
      background-color: yellow;
      backface-visibility: hidden; /*设置后面的可适度为看不见*/
    }
  </style>
</head>
<body style="background-color:#23d19d">
  <div id="box">
    <div class="bian zhi1"><img src="images/img1.jpeg" alt=""></div>
    <div class="bian zhi2"><img src="images/img2.jpeg" alt=""></div>
  </div>
</body>
</html>
```

**立方体**

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Cube</title>
  <style>
    img{
      width: 200px;
      height: 200px;
    }
    #box{
      perspective: 800px;
      transform-style: preserve-3d;
      transition: 5s infinite;
      transform: rotateX(0deg) rotateY(0deg);
    }
    .cube_box{
      width: 200px;
      height: 200px;
      margin: 100PX auto;
      position: relative;
      transform-style: preserve-3d;
      transition: 50s;
      transform:rotateX(0deg) rotateY(0deg);
    }
    .cube_box:hover{
      transform:rotateX(3600deg) rotateY(3600deg);
    }
    .cube{
      width: 200px;
      height: 200px;
      text-align: center;
      line-height: 200px;
      position: absolute;

    }
    /*原来这六个面的div是叠加在一起的通过旋转 移动来让他们形成正方体*/
    .left{
      transform:rotateY(90deg) translateZ(-100px);
    }
    .right{
      transform:rotateY(90deg) translateZ(100px);
    }
    .top{
      transform:rotateX(90deg) translateZ(100px) rotateZ(360deg);
    }
    .buttom{
      transform:rotateX(90deg) translateZ(-100px) rotateZ(180deg);
    }
    .back{
      transform:rotateX(0deg) translateZ(-100px) rotateZ(180deg);
    }
    .front{
      transform:rotateX(0deg) translateZ(100px);
    }
  </style>
</head>
<body style="background-color:#23d19d">
  <div id="box">
    <div class="cube_box" id="cube_box">
      <div class="cube front"><img src="images/img1.jpeg"></div>
      <div class="cube back"><img src="images/img2.jpeg"></div>
      <div class="cube left"><img src="images/img3.jpeg"></div>
      <div class="cube right"><img src="images/img4.jpeg"></div>
      <div class="cube top"><img src="images/img5.jpeg"></div>
      <div class="cube buttom"><img src="images/img6.jpeg"></div>
    </div>
  </div>
  <script type="text/javascript"src="js/index02.js"></script>
</body>  
</html>
```



## CSS3过渡效果

W3C标准中对css3的transition这是样描述的：“css的transition允许css的属性值在一定的时间区间内平滑地过渡。这种效果可以在鼠标单击、获得焦点、被点击或对元素任何改变中触发，并圆滑地以动画效果改变CSS的属性值。”

### 定义和用法

```
transition：[ transition-property ] || [ transition-duration ] || [ transition-timing-function ] || [ transition-delay ]
```

### transition 属性值

```
[ transition-property ]：检索或设置对象中的参与过渡的属性
[ transition-duration ]：检索或设置对象过渡的持续时间
[ transition-timing-function ]：检索或设置对象中过渡的动画类型
[ transition-delay ]：检索或设置对象延迟过渡的时间
```

### transition说明

复合属性。检索或设置对象变换时的过渡。
可以为同一元素的多个属性定义过渡效果。

```
transition:border-color .5s ease-in .1s, background-color .5s ease-in .1s, color .5s ease-in .1s;
```

```
transition-property: border-color, background-color, color;
transition-duration: .5s, .5s, .5s;
transition-timing-function: ease-in, ease-in, ease-in;
transition-delay: .1s, .1s, .1s;
```

如果定义了多个过渡的属性，而其他属性只有一个参数值，则表明所有需要过渡的属性都应用同一个参数值。据此可以对上面的例子进行缩写：

```
transition: all .5s ease-in .1s;
```

拆分方式：

```
transition-property: all;
transition-duration: .5s;
transition-timing-function: ease-in;
transition-delay: .1s;
```

### transition-property

transition-property是用来指定当元素其中一个属性改变时执行transition效果，其主要有以下几个值：none(没有属性改变)；all（所有属性改变）这个也是其默认值；indent（元素属性名）。当其值为none时，transition马上停止执行，当指定为all时，则元素产生任何属性值变化时都将执行transition效果，ident是可以指定元素的某一个属性值。

### transition-duration

transition-duration是用来指定元素 转换过程的持续时间，取值：<time>为数值，单位为s（秒）或者ms(毫秒),可以作用于所有元素，包括:before和:after伪元素。其默认值是0，也就是变换时是即时的。

### transition-timing-function

transition-timing-function的值允许你根据时间的推进去改变属性值的变换速率，transition-timing-function有6个可能值：
1、ease：（逐渐变慢）默认值，ease函数等同于贝塞尔曲线(0.25, 0.1, 0.25, 1.0).
2、linear：（匀速），linear 函数等同于贝塞尔曲线(0.0, 0.0, 1.0, 1.0).
3、ease-in：(加速)，ease-in 函数等同于贝塞尔曲线(0.42, 0, 1.0, 1.0).
4、ease-out：（减速），ease-out 函数等同于贝塞尔曲线(0, 0, 0.58, 1.0).
5、ease-in-out：（加速然后减速），ease-in-out 函数等同于贝塞尔曲线(0.42, 0, 0.58, 1.0)
6、cubic-bezier：（该值允许你去自定义一个时间曲线）， 特定的cubic-bezier曲线。 (x1, y1, x2, y2)四个值特定于曲线上点P1和点P2。所有值需在[0, 1]区域内，否则无效。
其是cubic-bezier为通过贝赛尔曲线来计算“转换”过程中的属性值，如下曲线所示，通过改变P1(x1, y1)和P2(x2, y2)的坐标可以改变整个过程的Output Percentage。初始默认值为default.

[获取贝塞尔方法工具](http://cubic-bezier.com/) 

### 案例

**百叶窗效果 blinds**

```
<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <title></title>
  <style type="text/css">
    * {
      margin: 0;
      padding: 0;
    }

    body {
      background-color: #cccccc;
      background: url(img/triangles.png) repeat;
    }

    .container {
      width: 805px;
      height: 320px;
      overflow: hidden;
      margin: 100px auto;
      -webkit-box-shadow: 0 0 5px #000;
    }

    .container li {
      width: 160px;
      display: block;
      position: relative;
      float: left;
      border-left: 1px solid #888;
      -webkit-box-shadow: 0 0 25px #000;
      -webkit-transition: all 0.5s;
    }

    .container ul:hover li {
      width: 40px;
    }

    .container ul li:hover {
      width: 640px;
    }

    .container li img {
      display: block;
    }

    .image_title {
      background: rgba(0, 0, 0, 0.5);
      position: absolute;
      left: 0;
      bottom: 0;
      width: 640px;
    }

    .image_title a {
      display: block;
      color: #fff;
      text-decoration: none;
      padding: 20px;
      font-size: 16px;
    }
  </style>
</head>

<body>
  <div class="container">
    <ul>
      <li>
        <div class="image_title">
          <a href="#">KungFu Panda</a>
        </div>
        <a href="#">
          <img src="img/img1.jpg">
        </a>
      </li>
      <li>
        <div class="image_title">
          <a href="#">Toy Story 2</a>
        </div>
        <a href="#">
          <img src="img/img2.jpg">
        </a>
      </li>
      <li>
        <div class="image_title">
          <a href="#">Wall-E</a>
        </div>
        <a href="#">
          <img src="img/img3.jpg">
        </a>
      </li>
      <li>
        <div class="image_title">
          <a href="#">Up</a>
        </div>
        <a href="#">
          <img src="img/img4.jpg">
        </a>
      </li>
      <li>
        <div class="image_title">
          <a href="#">Cars 2</a>
        </div>
        <a href="#">
          <img src="img/img5.jpg">
        </a>
      </li>
    </ul>
  </div>
</body>

</html>
```

**鼠标悬停 hover**

```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			figure{
				width: 295px;
				height: 246px;
				border:1px solid #cccccc;
				position: relative;
			}
			
			figure img{
				width: 285px;
				height:236px;
				position: absolute;
				left:5px;
				top:5px;
				transition: all 0.3s;
			}
			figure h3{
				position: absolute;
				top:50px;
				left:30%;
				text-align: center;
				transition: all 0.3s;	
				opacity: 0;		
			}
			figure span{
				position: absolute;
				top:90px;
				left:30%;
				text-align: center;
				transition: all 0.3s;	
				opacity: 0;		
			}
			figure a{
				position: absolute;
				bottom:50px;
				left:30%;
				text-align: center;
				transition: all 0.3s;
				opacity: 0;			
			}
			figure:hover h3{
				transform: translateY(-30px);
				opacity: 1;
				z-index: 99;			
			}
			figure:hover span{
				opacity: 1;
				transform: translateY(-30px);
				z-index: 99;			
			}
			figure:hover a{
				opacity: 1;
				transform: translateY(30px);
				z-index: 99;			
			}
			figure:hover img{
				width: 140px;
				height:115px;
				position: absolute;
				left:75px;
				top:75px;
				transition: all 0.3s;
			}
			.btn {
			  border: 1px solid #ff0000;
			  background-color: #ff0000;
			  text-align: center;
			  color: #ffffff;
			  padding: 5px 15px;
			}
			.btn:hover {
			  border-color: #ff3333;
			  background-color: #ff3d3d;
			  text-align: center;
			}
		</style>
	</head>
	<body>
		<figure>
			<img src="img/image01.jpg" />
			<figcaption>
				<h3>Web Design</h3>
			      <span>Rasty James</span> 
			      <a href="#" class="button">
			     	 <button class="btn ">Take a Look</button>
			      </a> 
			</figcaption>
		</figure>
	</body>
</html>

```



## CSS3动画

### 定义和用法

@keyframes 规则用于创建动画。
在 @keyframes 中规定某项 CSS 样式，就能创建由当前样式逐渐改为新样式的动画效果。
动画是使元素从一种样式逐渐变化为另一种样式的效果。
请用百分比来规定变化发生的时间，或用关键词 "from" 和 "to"，等同于 0% 和 100%, 0% 是动画的开始，100% 是动画的完成。
为了得到最佳的浏览器支持，应该始终定义 0% 和 100% 选择器
必须设置的项： 

- 规定动画的名称 
- 规定动画的时长

@keyframes test{ 
  from{} 
  to{} 
}
@keyframes test{ 
  0%{} 
  50%{} 
  ...... 
  100%{} 
}
animation: test 2s both

### 属性详解

```
animation: name duration timing-function delay iteration-count direction fill-mode play-state;
```

例：

```
animation: myanimation 2s linear 1s infinite forwards;
```

animation 属性是一个简写属性，用于设置动画属性：
```
animation-name
animation-duration
animation-timing-function
animation-delay
animation-iteration-count
animation-direction
animation-fill-mode
animation-play-state
```
- animation-name 动画名称

- animation-duration 动画指定需要多少秒或毫秒完成
  time 默认值为 0，意味着没有动画效果

- animation-timing-function 设置动画如何完成一个周期
 linear  匀速
   ease   先慢后快，结束前变慢     默认
   ease-in    低速开始
   ease-out  低速结束
   ease-in-out   低速开始和结束
   cubic-bezier(n,n,n,n)    在 cubic-bezier 函数中自己的值。可能的值是从 0 到 1 的数值
  
- animation-delay   动画在启动前的延迟间隔
  time 默认值为 0

- animation-iteration-count 动画的播放次数
 n  一个数字，定义播放多少次动画  默认值1
   infinite    动画无限次播放
  
- animation-direction  是否轮流反向播放动画
 normal 正常
   reverse  反向播放
   alternate 在奇数次（1、3、5...）正向播放，在偶数次（2、4、6...）反向播放
   alternate-reverse 在奇数次（1、3、5...）反向播放，在偶数次（2、4、6...）正向播放
  
- animation-fill-mode 当动画不播放时（当动画完成时，或当动画有一个延迟未开始播放时），要处于什么状态
 none 默认，播放完动画后，画面停在起始位置
   forwards  播放完动画，停在animation定义的最后一帧(保持最后一个属性值)
   backwards 如果设置了animation-delay，在开始到delay这段时间，画面停在第一帧。如果没有设置delay，画面是元素设置的初始值
   both 设置动画状态为动画结束或开始的状态（例如设置奇数播放为forwards状态，偶数播放为backwards状态）
  
- animation-play-state 动画是否正在运行或已暂停
 paused 指定暂停动画
   running 指定正在运行的动画，默认
   initial 设置属性为其默认值
   inherit 从父元素继承属性

### 案例

跑步，小车，自行车


## 媒体查询

### 定义和用法

**什么是媒体查询**

媒体查询可以让我们根据设备显示器的特性（如视口宽度、屏幕比例、设备方向：横向或纵向）为其设定CSS样式，媒体查询由媒体类型和一个或多个检测媒体特性的条件表达式组成。媒体查询中可用于检测的媒体特性有 width 、 height 和 color （等）。使用媒体查询，可以在不改变页面内容的情况下，为特定的一些输出设备定制显示效果。

**为什么响应式设计需要媒体查询**

如果没有CSS3的媒体查询模块，就不能针对设备特性（如视口宽度）设置特定的CSS样式

**如何在CSS文件中引入媒体查询**

媒体查询写在CSS样式代码的最后，CSS是层叠样式表，在同一特殊性下，靠后的的样式会重叠前面的样式

### 媒体查询的语法

```
<!-- link元素中的CSS媒体查询 -->
<link rel="stylesheet" media="(max-width: 800px)" href="example.css" />
<!-- 样式表中的CSS媒体查询 -->
<style>
@media (max-width: 600px) {
  .facet_sidebar {
    display: none;
  }
}
</style>
```

值得注意的是：当媒体查询为true时，其对应的样式表或样式规则就会遵循正常的级联规则进行应用。即使媒体查询返回false，<link> 标签指向的样式表也将会被下载(但是它们不会被应用)。

### 逻辑操作

and，且的关系，当所有的条件满足的时候返回true

```
//一个基本的媒体查询，即一个媒体属性和默认指定的all媒体类型
@media (min-width:700px){}

//如果你只想再横屏时候应用,你可以使用and操作符合并媒体属性
(min-width:700px)and(orientation:landscape){}

//如果你仅想在电视媒体上应用
@media tv and (min-width:700px) and (orientation:landscape){}
```

逗号分割列表，或的关系，只要有条件满足就返回ture

```
//如果你想在最小宽度为700像素或者横屏的手持设备上应用
@media (min-width:700px),handheld and (orientation:lanscape){}
```

not，类似于取反，最后参与运算的运算符

only，only关键字防止老旧的浏览器不支持带媒体属性的查询而应用到给定的样式 

### 设备类型
- screen 计算机屏幕（默认值）    
- tty  电传打字机以及使用等宽字符网格的类似媒介
- tv   电视类型设备（低分辨率、有限的屏幕翻滚能力）
- projection   放映机
- handheld  手持设备（小屏幕、有限的带宽）
- print  打印预览模式 / 打印页
- braille  盲人用点字法反馈设备
- aural 语音合成器
- all  适合所有设备


### 媒体查询参数

- width:浏览器可视宽度，
- height:浏览器可视高度，
- device-width:设备屏幕的宽度，
- device-height:设备屏幕的高度，
- orientation:检测设备目前处于横向还是纵向状态，
- aspect-ratio:检测浏览器可视宽度和高度的比例(例如：aspect-ratio:16/9)，
- device-aspect-ratio:检测设备的宽度和高度的比例，
- color:检测颜色的位数（例如：min-color:32就会检测设备是否拥有32位颜色），
- color-index:检查设备颜色索引表中的颜色（他的值不能是负数），
- monochrome:检测单色楨缓冲区域中的每个像素的位数（这个太高级，估计咱很少会用的到），
- resolution:检测屏幕或打印机的分辨率(例如：min-resolution:300dpi或min-resolution:118dpcm)，
- grid：检测输出的设备是网格的还是位图设备。

参考：https://www.cnblogs.com/lguow/p/9316598.html

### 案例

响应式网页设计

## Web字体

### CSS3 @font-face 规则

在 CSS3 之前，web 设计师必须使用已在用户计算机上安装好的字体。

通过 CSS3，web 设计师可以使用他们喜欢的任意字体。

当您您找到或购买到希望使用的字体时，可将该字体文件存放到 web 服务器上，它会在需要时被自动下载到用户的计算机上。

您“自己的”的字体是在 CSS3 @font-face 规则中定义的。

### 小例子

```
<style> 
@font-face {
    font-family: myFirstFont;
    src: url('Sansation_Light.ttf'),
         url('Sansation_Light.eot'); /* IE9+ */
    font-weight: bold;
}

div {
     font-family: myFirstFont;
}
</style>
```

### CSS3 字体描述符

下面的表格列出了能够在 @font-face 规则中定义的所有字体描述符：

| 描述符        | 值                                                           | 描述                                                         |
| :------------ | :----------------------------------------------------------- | :----------------------------------------------------------- |
| font-family   | *name*                                                       | 必需。规定字体的名称。                                       |
| src           | *URL*                                                        | 必需。定义字体文件的 URL。                                   |
| font-stretch  | normal/condensed/ultra-condensed/extra-condensed/semi-condensed/expanded/semi-expanded/extra-expanded/ultra-expanded | 可选。定义如何拉伸字体。默认是 "normal"。                    |
| font-style    | ormal/italic/oblique                                         | 可选。定义字体的样式。默认是 "normal"。                      |
| font-weight   | normal/bold/100/200/300/400/500/600/700/800/900              | 可选。定义字体的粗细。默认是 "normal"。                      |
| unicode-range | *unicode-range*                                              | 可选。定义字体支持的 UNICODE 字符范围。默认是 "U+0-10FFFF"。 |

### 案例

tabbar iconfont

## CSS3边框

### 定义

通过 CSS3，您能够创建圆角边框，向矩形添加阴影，使用图片来绘制边框 - 并且不需使用设计软件，比如 PhotoShop。

边框属性：

- border-radius
- box-shadow
- border-image

### CSS3圆角边框

```
div {
    border:2px solid;
    border-radius: 25px;
}
```

### CSS3 边框阴影

```
div {
		box-shadow: 10px 10px 5px #888888;
}
```

### CSS3 图片边框

通过 CSS3 的 border-image 属性，您可以使用图片来创建边框

```
div {
  -webkit-border-image:url(border.png) 30 30 round; /* Safari 5 */
  -o-border-image:url(border.png) 30 30 round; /* Opera */
  border-image:url(border.png) 30 30 round;
}
```

**定义和用法**

border-image 属性是一个简写属性，用于设置以下属性：

| 值                  | 描述                                                         |
| ------------------- | ------------------------------------------------------------ |
| border-image-source | 用在边框的图片的路径。                                       |
| border-image-slice  | 图片边框向内偏移。                                           |
| border-image-width  | 图片边框的宽度。                                             |
| border-image-outset | 边框图像区域超出边框的量。                                   |
| border-image-repeat | 图像边框是否应平铺(repeated)、铺满(rounded)或拉伸(stretched)。 |

**案例**

```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			*{padding: 0;margin: 0;}
			div{
				width: 300px;
				height: 100px;
				margin: 30px auto;
				border: 18px solid #f00;
				border-image-source: url(../img/borderimage.png);
				/*background-color: #f66;*/
				border-image-slice: 18 25 18 25;
				/*border-image-width:24px 1 10% 24px;*/
				border-image-width: 18px;
				border-image-outset: 18px;
				/*border-image-repeat: round;*/
				border-image-repeat: repeat;
			}
			div:nth-child(2){
				border-image: url(../img/border.png) 25 25 25 25/5px round;
			}
		</style>
	</head>
	<body>
		<div></div>
		<div></div>
	</body>
</html>
```



## CSS3背景

### 新的背景属性

CSS3 包含多个新的背景属性，它们提供了对背景更强大的控制。

| 属性              | 描述                     |
| ----------------- | ------------------------ |
| background-clip   | 规定背景的绘制区域。     |
| background-origin | 规定背景图片的定位区域。 |
| background-size   | 规定背景图片的尺寸。     |

### 案例

**多背景**

```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			*{padding: 0;margin: 0;}
			div{
				width: 800px;
				height: 600px;
				/*background-image: url(img/sky.jpg);
				background-repeat: no-repeat;
				background-position: center center;*/
				background-image: url(./img/flower-green.png),url(./img/flower-red.png),url(./img/sky.jpg);
				background-repeat: repeat-y, repeat-x, no-repeat;
				background-position: 90% 10%,30% 80%,center;
			}
		</style>
	</head>
	<body>
		<div>
			
		</div>
	</body>
</html>
```
**background-clip**
```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			*{
				padding: 0;
				margin: 0;
			}
			div{
				width: 400px;
				height: 300px;
				margin: 50px auto;
				background: url(../img/sky.jpg);
				padding: 20px;
				border: 10px dashed #ccc;

			}
			div:nth-child(1){
				-webkit-background-clip: content-box;
				-moz-background-clip: content-box;
				background-clip: content-box;
			}

			div:nth-child(2){
				-webkit-background-clip: padding-box;
				-moz-background-clip: padding-box;
				background-clip: padding-box;
			}

			div:nth-child(3){
				-webkit-background-clip: border-box;
				-moz-background-clip: border-box;
				background-clip: border-box;
				background-origin: border-box;
			}
		</style>
	</head>
	<body>
		<div >
			背景图片相关新增属性content-box
		</div>
		<div >
			背景图片相关新增属性padding-box
		</div>
		<div >
			背景图片相关新增属性border-box
		</div>
	</body>
</html>
```
**background-origin**
```
<!DOCTYPE html>
<html>
	<head>
		<meta charset="utf-8">
		<title></title>
		<style type="text/css">
			*{padding: 0;margin: 0;}
			div{
				width: 200px;
				height:200px;
				border: 10px dashed #f66;
				background: url(../img/flower-red.png) no-repeat;
				padding: 20px;

			}
			div:nth-child(1){
				background-origin: content-box;
			}
			div:nth-child(2){
				background-origin: padding-box;
			}
			div:nth-child(3){
				background-origin: border-box;
				background-size: 100% 100%;
			}
		</style>
	</head>
	<body>
		<div>
			背景图片放置位置content-box
		</div>
		<div>
			背景图片放置位置padding-box
		</div>
		<div>
			背景图片放置位置border-box
		</div>
	</body>
</html>
```



## CSS3文本

### 新的文本属性

| 属性                | 描述                                                      |
| ------------------- | --------------------------------------------------------- |
| hanging-punctuation | 规定标点字符是否位于线框之外。                            |
| punctuation-trim    | 规定是否对标点字符进行修剪。                              |
| text-align-last     | 设置如何对齐最后一行或紧挨着强制换行符之前的行。          |
| text-emphasis       | 向元素的文本应用重点标记以及重点标记的前景色。            |
| text-justify        | 规定当 text-align 设置为   "justify" 时所使用的对齐方法。 |
| text-outline        | 规定文本的轮廓。                                          |
| text-overflow       | 规定当文本溢出包含元素时发生的事情。                      |
| text-shadow         | 向文本添加阴影。                                          |
| text-wrap           | 规定文本的换行规则。                                      |
| word-break          | 规定非中日韩文本的换行规则。                              |
| word-wrap           | 允许对长的不可分割的单词进行分割并换行到下一行。          |

## CSS3颜色

CSS3允许我们使用新方法如RGB或HSL来声明颜色。另外，我们还能在这两个方法后边追加一个透明通道（分别是RGBA和HSLA）。

### 十六进制
```
nav ul li:nth-child(odd) a{
　color: #fe0208;
}
```

### RGB

```
nav ul li:nth-child(odd) a{
　color: rgb(254,2,8);
}　
```

### HSL

除了 RGB,CSS3还可使用HSL（色相、饱和度、亮度）模式来声明颜色。

HSL模式基于一个360º的色相环，如hsl(315,100%,60%)。第一个数字代表色相，60º为黄色，120º时为绿色，180º时为青色，240º时为蓝色，300º时为洋红色，360º时为红色。其后的两个值分别表示饱和度和亮度，值为百分比，用于改变基础的色相。如果想要更加饱满的颜色，则第二个值使用高一点的百分比即可。最后一个控制亮度，可在0%的全黑到100%的全白之间变化。

### 透明通道

HSL和RGB支持透明通道。CSS3还允许通过opacity声明来设置元素的透明度。该透明度的值也是一个介于0和1之间的小数。但是这种方式设置的透明度会对整个元素产生影响（元素的内容都会透明）。反之，使用HSLA或者RGBA则可以仅让元素的某些部分有透明效果。这样，一个元素可以带有HSLA透明效果，但内部的文字仍然不透明。

```
background-color: hsla(0,0,0，0.8)；
background-color: hsla(0,0%,100%，0.8)；
```



## CSS3多列布局

### 定义和用法

曾经有需要将一整段文本显示在多个栏位中，在CSS3出现以前，你必须将内容拆分到不同的标签中，然后分别设定样式。利用CSS3可以让我们将一段或多段内容分布到多列网格中

使用多栏布局时只能为所有栏指定一个统一的高度，栏与栏之间的宽也是一样的，另外也不能具体指定什么栏中显示什么内容，因此比较适合使用在显示文章内容的时候，不适合用于安排整个网页中由各元素组成的网页结构。

### 属性

**1、栏宽度属性column-width**
设定分栏布局中一个栏的宽度值；实际宽度会根据外层盒子的宽度有所调整（可能变大）。

**2、栏数量属性column-count**
设定分栏布局中的总栏数。

**3、columns属性：**
上述column-width和column-count的综合属性；
使用形式：columns: 栏宽值 栏目数；
实际表现上，当总宽度大于等于“栏宽x栏目数”时，栏目数固定，栏宽可能会有所调整（变大）。
当总宽度小于“栏宽x栏目数”时，栏目数会减少（保证栏宽不小于设定的栏宽）。

**4、栏间隙属性column-gap**
设定栏与栏之间的宽度值，默认是font-size大小（比如14px）

**5、栏分割线属性column-rule**
栏分割线属性，就是两栏之间的线，如果不设定默认就是“空的”，就没有分割线，只有间隙（gap）。
栏分割线属性类似边框线（但只是一条线），可以设定：线宽，线型，线色。
有如下几个属性：
column-rule-width：设定线宽，比如1px，5px；
column-rule-style：设定线型，比如solid，dashed，dotted；
column-rule-color：设定线色，比如red， #ff9966， rgb(200,100,0)

### 案例

```
<!DOCTYPE html>
<html lang="en">

    <head>
        <meta charset="UTF-8">
        <title>CSS3瀑布流</title>
        <meta name="viewport" content="width=device-width,initial-scale=1,maximum-scale=1,user-scalable=no">
        <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
        <style>
            * {
                margin: 0;
                padding: 0;
            }
            /*大层*/
            
            .container {
                width: 100%;
                margin: 0 auto;
            }
            /*瀑布流层*/
            .waterfall {
                -moz-column-count: 4;
                /* Firefox */
                -webkit-column-count: 4;
                /* Safari 和 Chrome */
                column-count: 4;
                -moz-column-gap: 0.5em;
                -webkit-column-gap: 0.5em;
                column-gap: 0.5em;
            }
            /*一个内容层*/            
            .item {
                padding: 0;
                margin: 0 0 1em 0;
                -moz-page-break-inside: avoid;
                -webkit-column-break-inside: avoid;
                break-inside: avoid;
                border: 1px solid #000;
            }
            
            .item img {
                width: 100%;
                margin-bottom: 10px;
            }
        </style>
    </head>

    <body>
        <div class="container">
            <div class="waterfall">
                <div class="item">
                    <img src="https://imgsa.baidu.com/baike/c0%3Dbaike72%2C5%2C5%2C72%2C24/sign=f3d4063328738bd4d02cba63c0e2ecb3/a2cc7cd98d1001e910616de1be0e7bec55e797fa.jpg">
                    <p>1 convallis timestamp</p>
                </div>

                <div class="item">
                    <img src="https://imgsa.baidu.com/baike/c0%3Dbaike92%2C5%2C5%2C92%2C30/sign=03948ea9b4315c60579863bdecd8a076/8326cffc1e178a825a6b5d1cfe03738da977e833.jpg">
                    <p>2 convallis timestamp 2 Donec a fermentum nisi. </p>
                </div>

                <div class="item">
                    <img src="https://imgsa.baidu.com/baike/c0%3Dbaike80%2C5%2C5%2C80%2C26/sign=3d645bf2d0ca7bcb6976cf7ddf600006/6d81800a19d8bc3efe5f64fb858ba61ea8d345af.jpg">
                    <p>3 Nullam eget lectus augue. Donec eu sem sit amet ligula faucibus suscipit. Suspendisse rutrum turpis quis nunc convallis quis aliquam mauris suscipit.</p>
                </div>

                <div class="item">
                    <img src="https://imgsa.baidu.com/baike/c0%3Dbaike180%2C5%2C5%2C180%2C60/sign=fbc3501b0a087bf469e15fbb93ba3c49/bf096b63f6246b60ea65dd24e3f81a4c510fa273.jpg">
                    <p> 4 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue. </p>
                </div>

                <div class="item">
                    <img src="https://imgsa.baidu.com/baike/c0%3Dbaike150%2C5%2C5%2C150%2C50/sign=9fe1d71697ef76c6c4dff379fc7f969f/b03533fa828ba61ed2efcd184634970a304e5987.jpg">
                    <p> 5 Donec a fermentum nisi. Integer dolor est, commodo ut sagittis vitae, egestas at augue.</p>
                </div>
            </div>
        </div>
    </body>

</html>
```



## CSS3渐变

### 定义

CSS3 渐变（gradients）可以让你在两个或多个指定的颜色之间显示平稳的过渡。

以前，你必须使用图像来实现这些效果。但是，通过使用 CSS3 渐变（gradients），你可以减少下载的时间和宽带的使用。此外，渐变效果的元素在放大时看起来效果更好，因为渐变（gradient）是由浏览器生成的。

CSS3 定义了两种类型的渐变（gradients）：

- **线性渐变（Linear Gradients）- 向下/向上/向左/向右/对角方向**
- **径向渐变（Radial Gradients）- 由它们的中心定义**

### CSS3 线性渐变

为了创建一个线性渐变，你必须至少定义两种颜色结点。颜色结点即你想要呈现平稳过渡的颜色。同时，你也可以设置一个起点和一个方向（或一个角度）。

#### 设置起点

background: linear-gradient(*direction*, *color-stop1*, *color-stop2, ...*);

**线性渐变 - 从上到下（默认情况下）**

```
#grad {
  background: -webkit-linear-gradient(red, blue); /* Safari 5.1 - 6.0 */
  background: -o-linear-gradient(red, blue); /* Opera 11.1 - 12.0 */
  background: -moz-linear-gradient(red, blue); /* Firefox 3.6 - 15 */
  background: linear-gradient(red, blue); /* 标准的语法 */
}
```

**线性渐变 - 从左到右**

```
#grad {
  background: -webkit-linear-gradient(left, red , blue); /* Safari 5.1 - 6.0 */
  background: -o-linear-gradient(right, red, blue); /* Opera 11.1 - 12.0 */
  background: -moz-linear-gradient(right, red, blue); /* Firefox 3.6 - 15 */
  background: linear-gradient(to right, red , blue); /* 标准的语法 */
}
```

**线性渐变 - 对角**

```
#grad {
  background: -webkit-linear-gradient(left top, red , blue); /* Safari 5.1 - 6.0 */
  background: -o-linear-gradient(bottom right, red, blue); /* Opera 11.1 - 12.0 */
  background: -moz-linear-gradient(bottom right, red, blue); /* Firefox 3.6 - 15 */
  background: linear-gradient(to bottom right, red , blue); /* 标准的语法 */
}
```

#### 使用角度

如果你想要在渐变的方向上做更多的控制，你可以定义一个角度，而不用预定义方向（to bottom、to top、to right、to left、to bottom right，等等）。

background: linear-gradient(*angle*, *color-stop1*, *color-stop2*);

角度是指水平线和渐变线之间的角度，逆时针方向计算。换句话说，0deg 将创建一个从下到上的渐变，90deg 将创建一个从左到右的渐变。

![img](https://www.runoob.com/wp-content/uploads/2014/07/7B0CC41A-86DC-4E1B-8A69-A410E6764B91.jpg)

但是，请注意很多浏览器(Chrome,Safari,fiefox等)的使用了旧的标准，即 0deg 将创建一个从左到右的渐变，90deg 将创建一个从下到上的渐变。换算公式 **90 - x = y** 其中 x 为标准角度，y为非标准角度。

```
#grad {
  background: -webkit-linear-gradient(180deg, red, blue); /* Safari 5.1 - 6.0 */
  background: -o-linear-gradient(180deg, red, blue); /* Opera 11.1 - 12.0 */
  background: -moz-linear-gradient(180deg, red, blue); /* Firefox 3.6 - 15 */
  background: linear-gradient(180deg, red, blue); /* 标准的语法 */
}
```

#### 使用多个颜色节点

```
#grad {
  background: -webkit-linear-gradient(red, green, blue); /* Safari 5.1 - 6.0 */
  background: -o-linear-gradient(red, green, blue); /* Opera 11.1 - 12.0 */
  background: -moz-linear-gradient(red, green, blue); /* Firefox 3.6 - 15 */
  background: linear-gradient(red, green, blue); /* 标准的语法 */
}
```

```
#grad {
  /* Safari 5.1 - 6.0 */
  background: -webkit-linear-gradient(left,red,orange,yellow,green,blue,indigo,violet);
  /* Opera 11.1 - 12.0 */
  background: -o-linear-gradient(left,red,orange,yellow,green,blue,indigo,violet);
  /* Firefox 3.6 - 15 */
  background: -moz-linear-gradient(left,red,orange,yellow,green,blue,indigo,violet);
  /* 标准的语法 */
  background: linear-gradient(to right, red,orange,yellow,green,blue,indigo,violet); 
}
```

#### 使用透明度

CSS3 渐变也支持透明度（transparent），可用于创建减弱变淡的效果。

为了添加透明度，我们使用 rgba() 函数来定义颜色结点。rgba() 函数中的最后一个参数可以是从 0 到 1 的值，它定义了颜色的透明度：0 表示完全透明，1 表示完全不透明。

```
#grad {
  background: -webkit-linear-gradient(left,rgba(255,0,0,0),rgba(255,0,0,1)); /* Safari 5.1 - 6 */
  background: -o-linear-gradient(right,rgba(255,0,0,0),rgba(255,0,0,1)); /* Opera 11.1 - 12*/
  background: -moz-linear-gradient(right,rgba(255,0,0,0),rgba(255,0,0,1)); /* Firefox 3.6 - 15*/
  background: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1)); /* 标准的语法 */
}
```

#### 重复的线性渐变

```
#grad {
  /* Safari 5.1 - 6.0 */
  background: -webkit-repeating-linear-gradient(red, yellow 10%, green 20%);
  /* Opera 11.1 - 12.0 */
  background: -o-repeating-linear-gradient(red, yellow 10%, green 20%);
  /* Firefox 3.6 - 15 */
  background: -moz-repeating-linear-gradient(red, yellow 10%, green 20%);
  /* 标准的语法 */
  background: repeating-linear-gradient(red, yellow 10%, green 20%);
}
```

### CSS3 径向渐变

径向渐变由它的中心定义。

为了创建一个径向渐变，你也必须至少定义两种颜色结点。颜色结点即你想要呈现平稳过渡的颜色。同时，你也可以指定渐变的中心、形状（圆形或椭圆形）、大小。默认情况下，渐变的中心是 center（表示在中心点），渐变的形状是 ellipse（表示椭圆形），渐变的大小是 farthest-corner（表示到最远的角落）。

background: radial-gradient(*center, shape size, start-color, ..., last-color*);

**径向渐变 - 颜色结点均匀分布（默认情况下）**

```
#grad {
  background: -webkit-radial-gradient(red, green, blue); /* Safari 5.1 - 6.0 */
  background: -o-radial-gradient(red, green, blue); /* Opera 11.6 - 12.0 */
  background: -moz-radial-gradient(red, green, blue); /* Firefox 3.6 - 15 */
  background: radial-gradient(red, green, blue); /* 标准的语法 */
}
```

**径向渐变 - 颜色结点不均匀分布**

```
#grad {
  background: -webkit-radial-gradient(red 5%, green 15%, blue 60%); /* Safari 5.1 - 6.0 */
  background: -o-radial-gradient(red 5%, green 15%, blue 60%); /* Opera 11.6 - 12.0 */
  background: -moz-radial-gradient(red 5%, green 15%, blue 60%); /* Firefox 3.6 - 15 */
  background: radial-gradient(red 5%, green 15%, blue 60%); /* 标准的语法 */
}
```

#### 设置形状

shape 参数定义了形状。它可以是值 circle 或 ellipse。其中，circle 表示圆形，ellipse 表示椭圆形。默认值是 ellipse。

```
#grad {
  background: -webkit-radial-gradient(circle, red, yellow, green); /* Safari 5.1 - 6.0 */
  background: -o-radial-gradient(circle, red, yellow, green); /* Opera 11.6 - 12.0 */
  background: -moz-radial-gradient(circle, red, yellow, green); /* Firefox 3.6 - 15 */
  background: radial-gradient(circle, red, yellow, green); /* 标准的语法 */
}
```

#### 不同尺寸大小关键字的使用

size 参数定义了渐变的大小。它可以是以下四个值：

- **closest-side**
- **farthest-side**
- **closest-corner**
- **farthest-corner**

```
#grad1 {
  /* Safari 5.1 - 6.0 */
  background: -webkit-radial-gradient(60% 55%, closest-side,blue,green,yellow,black); 
  /* Opera 11.6 - 12.0 */
  background: -o-radial-gradient(60% 55%, closest-side,blue,green,yellow,black);
  /* Firefox 3.6 - 15 */
  background: -moz-radial-gradient(60% 55%, closest-side,blue,green,yellow,black);
  /* 标准的语法 */
  background: radial-gradient(60% 55%, closest-side,blue,green,yellow,black);
}
 
#grad2 {
  /* Safari 5.1 - 6.0 */
  background: -webkit-radial-gradient(60% 55%, farthest-side,blue,green,yellow,black);
  /* Opera 11.6 - 12.0 */ 
  background: -o-radial-gradient(60% 55%, farthest-side,blue,green,yellow,black);
  /* Firefox 3.6 - 15 */
  background: -moz-radial-gradient(60% 55%, farthest-side,blue,green,yellow,black);
  /* 标准的语法 */
  background: radial-gradient(60% 55%, farthest-side,blue,green,yellow,black);
}
```

#### 重复的镜像渐变

```
#grad {
  /* Safari 5.1 - 6.0 */
  background: -webkit-repeating-radial-gradient(red, yellow 10%, green 15%);
  /* Opera 11.6 - 12.0 */
  background: -o-repeating-radial-gradient(red, yellow 10%, green 15%);
  /* Firefox 3.6 - 15 */
  background: -moz-repeating-radial-gradient(red, yellow 10%, green 15%);
  /* 标准的语法 */
  background: repeating-radial-gradient(red, yellow 10%, green 15%);
}
```


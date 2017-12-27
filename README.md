# HTML بالعربي

# مرجع مبسّط باللغة العربية للـ HTML. {#html}

## فهرس المحتويات

* [صفحة مبدئية](#minimal-page)
* [رأس الصفحة](#head)
* [تنسيقات النصوص](#text-content)
  * [العناوين](#headings)
  * [الفقرات](#paragraphs)
  * [التنسيقات](#formatting)
  * [الإقتباسات](#quotes)
* [المحتوى](#content)
  * [الروابط](#links)
  * [الصور](#images)
  * [الكتل](#blocks)
* [القوائم](#lists)
  * [القوائم الغير مرتبة](#unordered-list)
  * [القوائم المرتبة](#ordered-list)
  * [قوائم التعريف](#definition-list)
* [الجداول](#tables)
  * [الجداول البسيطة](#basic-table)
  * [الجداول المتقدمة](#advanced-table)
* [النماذج](#forms)
* [أوسمة HTML5](#html5-semantic)
  * [تخطيط الصفحة](#page-layout)
  * [العناصر الجديدة](#new-العنصرs)

## صفحة مبدئية مع دعم للغة العربية واتجاه من اليمين لليسار

```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
    <head>
        <meta charset="UTF-8">
        <title>عنوان الصفحة</title>
    </head>
    <body>
        <!-- محتوى الصفحة -->
    </body>
</html>
```

## رأس الصفحة

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>عنوان الصفحة</title>
    <base href="base-url">
    <meta name="keywords" content="keywords">
    <meta name="description" content="description">
    <meta name="author" content="name">
    <meta http-equiv="refresh" content="10">
    <link href="style.css" rel="stylesheet" type="text/css">
    <style type="text/css">
        /* CSS code */
    </style>
    <script src="script.js"></script>
    <script>
        // Javascript code
    </script>
</head>
```

| الوسم | العنصر |
| --- | --- |
| **title** | عنوان الصفحة الظاهر على تبويب مستعرض الإنترنت |
| **base** | base url for all links |
| **link** | link to external source |
| **style** | CSS inside HTML page |
| **script** | Javascript code |
| **meta** | metadata |
| **meta** _http-equiv_="refresh" _content_="10" | auto-refresh page in 10s |

## تنسيقات النصوص

### العناوين

```html
<h1>عنوان رئيسي</h1>
<!-- إلخ -->
<h6>عنوان من الدرجة السادسة</h6>
```

| الوسم | العنصر |
| --- | --- |
| **h1** | عنوان رئيسي |
| **h6** | عنوان أقل أهمية |

### الفقرات

```html
<p>فقرة.<br/>
سطر جديد.</p>
<p>فقرة أخرى.</p>
<hr/>
<p>لاحظ الخط الأفقي فوق هذا العنصر.</p>
```

| الوسم | العنصر |
| --- | --- |
| **p** | فقرة |
| **br** | سطر جديد |
| **hr** | خط أفقي |

### التنسيقات

```html
<em>التنسيقات</em> في صفحات الويب <strong>مهمة للغاية</strong> !
(س+ع)<sup>٢</sup> = س<sup>٢</sup> + ع<sup>٢</sup> + ٢سع
```

| الوسم | العنصر |
| --- | --- |
| **sub** | subscript |
| **sup** | superscript |
| **em** | emphasize |
| **strong** | important |
| **mark** | highlighted |
| **small** | small |
| **i** | italic |
| **b** | bold |

### الإقتباسات

```html
<cite>This book</cite> was written by this author.
<q cite="url">quotation</q>
<blockquote cite="url">
Lorem ipsum<br/>
Lorem ipsum
</blockquote>
```

| الوسم | العنصر |
| --- | --- |
| **cite** | title of a work |
| **q** | inline quotation |
| **blockquote** | quotation |

## المحتوى

### الروابط

```html
<a href="url">link</a>
<a href="url" target=_blank>open in a new window</a>

<a href="#comments">watch comments</a>
<h2 id="comments">comments</h2>
```

| الوسم | العنصر |
| --- | --- |
| **a** | hyperlink |

### الصور

```html
<img src="image.png" alt="description" width="300" height="200">
```

| الوسم | العنصر |
| --- | --- |
| **img** | image |

### الكتل

```html
<div>block</div>
<span>inline</span>
```

| الوسم | العنصر |
| --- | --- |
| **div** | block-level العنصر |
| **span** | inline العنصر |

## القوائم

### القوائم الغير مرتبة

```html
<ul>
    <li>item</li>
    <li>item</li>
    <li>item</li>
</ul>
```

| الوسم | العنصر |
| --- | --- |
| **ul** | unordered list |
| **li** | list item |

### القوائم المرتبة

```html
<ol>
    <li>first</li>
    <li>second</li>
    <li>third</li>
</ol>
```

| الوسم | العنصر |
| --- | --- |
| **ol** | ordered list |
| **li** | list item |

### قوائم التعريف

```html
<dl>
    <dt>term</dt><dd>definition</dd>
    <dt>term</dt><dd>definition</dd>
    <dt>term</dt><dd>definition</dd>
</dl>
```

| الوسم | العنصر |
| --- | --- |
| **dl** | definition list |
| **dt** | term |
| **dd** | definition |

## الجداول

### الجداول البسيطة

```html
<table>
<tr>
    <th>heading 1</th>
    <th>heading 2</th>
</tr>
<tr>
    <td>line 1, column 1</td>
    <td>line 1, column 2</td>
</tr>
<tr>
    <td>line 2, column 1</td>
    <td>line 2, column 2</td>
</tr>
</table>
```

| الوسم | العنصر |
| --- | --- |
| **table** | table |
| **tr** | table row |
| **th** | table heading |
| **td** | table cell |

### الجداول المتقدمة

```html
<table>
<caption>caption</caption>
<colgroup>
    <col span="2" style="...">
    <col style="...">
</colgroup>
<thead>
    <tr>
        <th>heading 1</th>
        <th>heading 2</th>
        <th>heading 3</th>
    </tr>
</thead>
<tfoot>
    <tr>
        <th>footer 1</th>
        <th>footer 2</th>
        <th>footer 3</th>
    </tr>
</tfoot>
<tbody>
    <tr>
        <td>line 1, column 1</td>
        <td>line 1, column 2</td>
        <td>line 1, column 3</td>
    </tr>
    <tr>
        <td>line 2, column 1</td>
        <td>line 2, column 2</td>
        <td>line 2, column 3</td>
    </tr>
</tbody>
</table>
```

| الوسم | العنصر |
| --- | --- |
| **caption** | caption |
| **colgroup** | defines groups of columns |
| **col** | defines column's properties |
| **thead** | groups headings together |
| **tfoot** | groups footers together |
| **tbody** | groups other rows |

## النماذج

```html
<form action="url" method="post">
    <fieldset>
        <legend>Who are you ?</legend>
        <label>Login :<input type="text" name="login"></label><br/>
        <label for="pswd">Password :</label><input type="password" name="password" id="pswd"><br/>
        <input type="radio" name="sex" value="male">Male<br/>
        <input type="radio" name="sex" value="female">Female<br/>
    </fieldset>

    <label>Your favorite color : <select name="color">
        <option>red</option>
        <option>green</option>
        <option>blue</option>
    </select></label>

    <input type="checkbox" name="available" value="monday">Monday<br/>
    <input type="checkbox" name="available" value="tuesday">Tuesday<br/>

    <textarea name="comments" rows="10" cols="30" placeholder="Write your comments here"><textarea/>

    <input type="submit" value="Button text">
</form>
```

| الوسم | العنصر |
| --- | --- |
| **form** | form |
| **label** | label for input |
| **fieldset** | group inputs together |
| **legend** | legend for fieldset |
| **input** type="_text_" | text input |
| **input** type="_password_" | password input |
| **input** type="_radio_" | radio button |
| **input** type="_checkbox_" | checkbox |
| **input** type="_submit_" | send form |
| **select** | drop-down list |
| **option** | drop-down list item |
| **optgroup** | group of drop-down list items |
| **datalist** | autocompletion list |
| **textarea** | large text input |

## أوسمة HTML5

### تخطيط الصفحة

```html
<header>My website</header>
<nav>
    <a href="page1">Page 1</a>
    <a href="page2">Page 2</a>
    <a href="page3">Page 3</a>
</nav>

<section>
    Hello everybody, Welcome to my website !
</section>

<article>
    <header>
        <h2>Title</h2>
    </header>
    <p>
        My article
    </p>
</article>

<aside>
    Writen by me
</aside>

<section id="comments">
    <article>Comment 1</article>
    <article>Comment 2</article>
</section>

<footer>
Copyright notice
</footer>
```

| الوسم | العنصر |
| --- | --- |
| **header** | header of document or section |
| **footer** | footer of document or section |
| **section** | section |
| **article** | article, forum post, blog post, comment |
| **aside** | aside content related to surrounding content |
| **nav** | navigation links |

### العناصر الجديدة

```html
<figure>
    <img src="image.png" alt="figure 1">
    <figcaption>Figure 1</figcaption>
</figure>

<details>
    <summary>Declaration of M. X on <time datetime="2013-12-25">Christmas day</time></summary>
    <p>M. X said...</p>
</details>

Downloading progress : <progress value="53" max="100"></progress>
Disk space : <meter value="62" min="10" max="350"></meter>
```

| الوسم | العنصر |
| --- | --- |
| **figure** | an illustration |
| **figcaption** | caption of a figure العنصر |
| **details** | details that can be shown or hidden |
| **summary** | visible heading of a details العنصر |
| **progress** | progress of a task |
| **meter** | display a gauge |
| **time** | machine-readable time indication |

&lt;/div&gt;


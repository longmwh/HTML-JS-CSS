
[head标签](https://developer.mozilla.org/zh-CN/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML)


学习目的：学习head标签，它的目的是什么，包含哪些元素以及它对页面有什么影响  

head标签是/<head/> 元素的内容。不像/<body/> 元素的内容可以显示在浏览器中，head的内容不会再浏览器中显示，它的作用是包含一些页面的元数据  


meta 标签  
charset 指定文档中的字符编码  
name 指定了meta元素的类型；说明改元素包含了什么类型的信息  
content 指定了实际的元数据内容  


在搜索引擎中description的使用  
    <meta name="description" content="The Mozilla Developer Network (MDN) provides
    information about Open Web technologies including HTML, CSS, and APIs for both
    Web sites and HTML5 Apps. It also documents Mozilla products, like Firefox OS.">  

这里content的内容会显示在网页标题的下面，作为对网页的描述，可以让用户提前了解到网页的内容  


自定义图标  
    <link rel="shortcut icon" href="favicon.ico" type="image/x-icon">  


在HTML中应用CSS和JavaScript  

    <link rel="stylesheet" href="my-css-file.css">   

<link>元素经常位于文档的头部。这个link元素有2个属性，rel="stylesheet"表明是文档的样式表，而href包含了样式表文件的路径;  

    <script src="my-js-file.js"><script>

<script>部分没有必要非要放在文档头部；实际上把它放在文档的尾部（在</body>标签之前）是一个很好的选择，可以确保在加载脚本之前浏览器已经解析了HTML内容（如果脚本加载某个不存在的元素，浏览器会报错）  
脚本也可以放在<script>中，而不是指向外部脚本文件.  

为文档设定主语言  
    <html lang="en-US">  
    <p>Janpanese example: <span lang="jp">ご飯が熱い。</span>.</p>  


## Dynalist Grabber：把任何网页的标题和 URL 快速抓取到 Dynalist/Workflowy

<script>
window.location.replace("https://pimgeek.github.io/pub/dynalist-grabber.html");
</script>

如果这是你第一次听说 Dynalist 和 Workflowy 这类工具，那么请借助我撰写的 [推荐 Dynalist.io 大纲笔记整理工具](https://www.zhihu.com/question/20491194/answer/87957399) 和 [Workflowy 快速上手教程](https://zhuanlan.zhihu.com/p/26824614) 做一些基本的了解，很多笔记管理爱好者用过它以后，都觉得爱不释手。

**--- 下面是 Dynalist Grabber 的用法说明 ---**

把下面的【抓取到 Dynalist/Workflowy】按钮拖拽或添加到浏览器书签栏，即可使用。

<div>
<p><a id="bookmarklet" style="border:2px solid dimgray;border-radius:5px;padding:3px;background-color:silver;" href="javascript:!function(){(function(){function%20o(o){return%20o.replace(/%26/g,%22%26amp;amp;%22).replace(/%3C/g,%22%26amp;lt;%22).replace(/%3E/g,%22%26amp;gt;%22).replace(/%22/g,%22%26quot;%22).replace(/(\n)/g,%22%26%2310;%22)}var%20e=%22https://workflowy.com/%23%22,n=o(document.title),t=o(location.href)+%22%20%22,r=o(window.getSelection().toString()),l=r.search(/[.;:%3F!。；：？！\r\n]/),i=(r.substring(0,l+1),location.href.indexOf(%22workflowy.com/%23%22)),a=!!window.chrome;if(i!==-1)var%20n=%22%26lt;i%26gt;参见%26quot;%22+n.replace(/%20-%20WorkFlowy$/,%22%22)+%22%26quot;%26lt;/i%26gt;%22;var%20c='%3C%3Fxml%20version=%221.0%22%3F%3E%3Copml%20version=%222.0%22%3E%20%20%3Chead%3E%20%20%20%20%3CownerEmail%3Epimgeek%40swarma.org%3C/ownerEmail%3E%20%20%3C/head%3E%20%20%3Cbody%3E%20%20%20%20%3Coutline%20text=%22['+n+%22](%22+t+')%22%20_note=%22'+r+'%22%20/%3E%20%20%3C/body%3E%3C/opml%3E';if(a%26%26c.length%3E2e3)window.open(e+%22/%3Fq=%22+encodeURIComponent(c));else{if(null===prompt(%22%20请复制下面的内容（Ctrl+C%20或%20Command+C），%20\n\n%20然后粘贴到%20Workflowy%20/%20Dynalist%20中。%20\n%22,c))return;i!==-1%26%26(location.href=e)}})()}();">抓取到 Dynalist/Workflowy</a></p>
</div>

在需要抽取标题和 URL 的网页上，先选中一段文字（不要取消选择），然后找到书签栏上的【抓取到 Dynalist/Workflowy】，即可获取 OPML 代码，最后把这段代码复制后粘贴到 Dynalist/Workflowy 列表中即可。

注：即使不选中任何文字，也可以抓取网页的标题和 URL；如果选中文字，则会填充到新增条目的笔记编辑区域。

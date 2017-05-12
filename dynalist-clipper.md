## Dynalist Clipper：把任何网页的标题和 URL 快速抓取到 Dynalist/ Workflowy

如果这是你第一次听说 Dynalist 和 Workflowy 这类工具，那么请借助我撰写的 [推荐 Dynalist.io 大纲笔记整理工具](https://www.zhihu.com/question/20491194/answer/87957399) 和 [Workflowy 快速上手教程](https://zhuanlan.zhihu.com/p/26824614) 做一些基本的了解，很多笔记管理爱好者用过它以后，都觉得爱不释手。

**--- 下面是 Dynalist Clipper 的用法说明 ---**

把下面的【抓取到 Dynalist/Workflowy】按钮拖拽或添加到浏览器书签栏，即可使用。

<div>
<p><a id="bookmarklet" style="border:2px solid dimgray;border-radius:5px;padding:3px;background-color:silver;" href="javascript:void%20function(){(function(){function%20e(e){var%20o=e.replace(/%26/g,%22%26amp;amp;%22).replace(/%3C/g,%22%26amp;lt;%22).replace(/%3E/g,%22%26amp;gt;%22).replace(/%22/g,%22%26quot;%22).replace(/(\n)/g,%22%26%2310;%22);return%20o}var%20o=%22https://workflowy.com/%23%22,t=e(document.title),n=e(location.href)+%22%20%22,l=e(window.getSelection().toString()),r=l.search(/[.;:%3F!。；：？！\r\n]/),i=l.substring(0,r+1),a=location.href.indexOf(%22workflowy.com/%23%22),c=!!window.chrome;if(-1!==a)var%20t=%22%26lt;i%26gt;参见%26quot;%22+t.replace(/%20-%20WorkFlowy$/,%22%22)+%22%26quot;%26lt;/i%26gt;%22;var%20u='%3C%3Fxml%20version=%221.0%22%3F%3E%3Copml%20version=%222.0%22%3E%20%20%3Chead%3E%20%20%20%20%3CownerEmail%3Eusername%40workflowy.com%3C/ownerEmail%3E%20%20%3C/head%3E%20%20%3Cbody%3E%20%20%20%20%3Coutline%20text=%22'+i+'%22%20%3E%20%20%20%20%20%20%3Coutline%20text=%22关注的重点%22%20_note=%22'+l+'%22%20/%3E%20%20%20%20%20%20%3Coutline%20text=%22关注的理由%22%20_note=%22我为何会收藏这个网址？%22%20/%3E%20%20%20%20%20%20%3Coutline%20text=%22传送门%22%20%3E%20%20%20%20%20%20%20%20%3Coutline%20text=%22'+t+'%22%20_note=%22'+n+'%22%20/%3E%3C/outline%3E%20%20%20%20%3C/outline%3E%20%20%3C/body%3E%3C/opml%3E';if(c%26%26u.length%3E2e3)window.open(%22%22+o+%22/%3Fq=%22+encodeURIComponent(u));else{var%20m=prompt(%22%20%20请复制下列文字%20(Ctrl%20+%20C)%20或%20(Cmd%20+%20C)%20\n\n%20%20并打开%20Workflowy%20页签粘贴为新的笔记条目\n%22,u);if(null===m)return;-1!==a%26%26(location.href=o)}})()}();">抓取到 Dynalist/Workflowy</a></p>
</div>

在需要抽取标题和 URL 的网页上，先选中一段文字（不要取消选择），然后找到书签栏上的【抓取到 Dynalist/Workflowy】，即可获取 OPML 代码，最后把这段代码复制后粘贴到 Dynalist / Workflowy 即可。

注：即使不选中任何文字，也可以抓取网页的标题和 URL；如果选中文字，则会填充到新增条目的笔记编辑区域。

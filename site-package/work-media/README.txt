如何添加作品
=============

1. 把你的图片、视频文件复制到这个 work-media 文件夹里（和 manifest.js 放在一起）。

2. 打开 manifest.js，在 window.WORK_ITEMS = [ ... ] 的方括号里，
   给每个文件加一行，例如：

     { type: 'image', src: 'work-media/我的海报设计.jpg' },
     { type: 'video', src: 'work-media/品牌宣传片.mp4' },

   type 填 'image' 或 'video'，src 填文件名（要和你放进文件夹的文件名完全一致）。

3. 保存 manifest.js，刷新网页，作品就会按你列的顺序显示在"work"页面里。

注意：
- index.html 和 work-media 文件夹必须放在一起，不要拆开或改名。
- 直接双击 index.html 用浏览器打开就可以看效果；如果作品不显示，
  换成 Chrome 打开一般都没问题（部分浏览器对本地文件读取比较严格）。
- 视频建议用 mp4 格式，体积别太大（网页视频不会像图片一样被压缩）。

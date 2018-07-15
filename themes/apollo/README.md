## 註: 此版本的 hexo-theme-apollo 是從 [原 repo](https://github.com/pinggod/hexo-theme-apollo/) fork 而來
- 因為 jade 這個專案已經整個改名，並轉換為 pug 了
- 有許多 jade 相關的套件 (像是 hexo-renderer-jade) 已經年久失修，所以這邊做了一個 pug 版本
- 原專案 hexo-theme-apollo 目前也不收任何 PR (所以現在 fork 400 多個)，對 hexo-theme-apollo-pug 有興趣可以發 issue (或直接 fork 走)

## 修改內容：
- 將原本的所有 `*.jade` 檔案都 rename 成 `*.pug`
- pug 在 `extend` 和 `include` 時都要強制加上副檔名
  ![](https://i.imgur.com/YEaktI9.png)
- 下面的安裝 script 也有更新，改成安裝 `hexo-renderer-pug`，以及 hexo 本身慣用的 yarn

## 安装
``` bash
hexo init BLOG
cd BLOG
yarn add hexo-renderer-pug hexo-generator-feed hexo-generator-sitemap hexo-browsersync hexo-generator-archive
git clone https://github.com/alxtz/hexo-theme-apollo-pug themes/apollo
```

## License

MIT

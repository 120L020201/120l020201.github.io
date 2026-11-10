# Xiang Li 的个人主页

极简静态个人主页，只展示姓名和邮箱。适配手机，无依赖、无构建步骤、不收集访客数据。

网站地址：<https://120l020201.github.io/>  
GitHub 仓库：<https://github.com/120L020201/120l020201.github.io>

## 填写姓名和邮箱

用文本编辑器打开 `profile.js`，修改引号内的两项内容：

```js
window.PROFILE = {
  name: "Xiang Li",
  email: "your.email@example.com",
};
```

将示例邮箱换成你的真实邮箱后，页面会显示邮箱地址，点击即可打开访客的邮件应用。
示例邮箱暂不生成链接，页面会显示 `Email to be added`。

双击 `index.html` 即可在浏览器中预览。

## 发布到 GitHub Pages

1. 在 GitHub 创建公开仓库，名字填写 `你的GitHub用户名.github.io`。如果该仓库已经存在，先查看其中的内容，避免覆盖已有网站。
2. 将本文件夹中的 `index.html`、`profile.js` 和 `.nojekyll` 上传到仓库根目录，提交到 `main` 分支。可以一并上传本说明文件。
3. 打开仓库的 **Settings → Pages**，将 **Source** 设为 **Deploy from a branch**，选择 **main** 和 **/(root)**，点击 **Save**。
4. 等待部署完成后，访问 `https://你的GitHub用户名.github.io/`。Pages 设置页也会显示网站链接。

以后只需在 GitHub 修改 `profile.js` 并提交，网站就会自动重新发布。

也可以使用普通仓库名（例如 `personal-homepage`），对应网址为 `https://你的GitHub用户名.github.io/personal-homepage/`。

官方说明：[创建 GitHub Pages 站点](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site)。

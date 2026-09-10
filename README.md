# 个人简历网站

这是一个无需安装依赖的静态单页简历，可直接部署到 GitHub Pages。

## 1. 修改内容

打开 `index.html`，搜索方括号 `[`，依次替换姓名、职位、城市、经历、项目、教育背景和技能。随后替换邮箱、GitHub、LinkedIn 链接，以及头像中的 `YN` 首字母。

本地预览时，直接双击 `index.html` 即可在浏览器中打开。

## 2. 部署到 GitHub Pages

1. 登录 GitHub，创建一个公开仓库。若希望网址是 `用户名.github.io`，仓库名也必须是 `用户名.github.io`；否则可以使用任意仓库名。
2. 将本文件夹中的 `index.html` 上传到仓库根目录并提交。
3. 打开仓库的 **Settings → Pages**。
4. 在 **Build and deployment** 中，将 **Source** 设为 **Deploy from a branch**。
5. 将分支选为 `main`，目录选为 `/ (root)`，点击 **Save**。
6. 等待 GitHub 完成发布。用户主页仓库的网址通常是 `https://用户名.github.io/`；普通仓库的网址通常是 `https://用户名.github.io/仓库名/`。

以后只需修改并提交 `index.html`，GitHub Pages 会自动更新网站。

## 3. 可选：使用 Git 命令上传

```bash
git init
git add index.html README.md
git commit -m "Add personal resume site"
git branch -M main
git remote add origin https://github.com/你的用户名/你的仓库名.git
git push -u origin main
```

执行后再按上面的 GitHub Pages 设置步骤开启发布。

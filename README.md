# 出城进城

一个可以直接在网页中游玩的平面策略小游戏。玩家和三个电脑角色通过石头剪刀布决定行动次数，在“玩家的城、电脑A的城、电脑B的城、电脑C的城、城外”之间移动、攻击、治疗，目标是存活并击败其他所有角色。

## 在线部署到 GitHub Pages

这个项目是纯静态网页，不需要构建步骤。GitHub Pages 可以直接发布根目录。

### 文件说明

- `index.html`：网站入口，会自动跳转到游戏页面。
- `outputs/chucheng-jincheng.html`：游戏本体。
- `outputs/assets/`：地图、棋子、按钮与特效的像素 PNG 素材；必须保持此目录结构。
- `.nojekyll`：让 GitHub Pages 按普通静态文件发布，不经过 Jekyll 处理。

## GitHub 网页端发布步骤

1. 在 GitHub 新建一个仓库，例如 `chucheng-jincheng`。
2. 打开仓库页面，点击 **Add file** -> **Upload files**。
3. 上传本项目中的 `index.html`、`.nojekyll`、`README.md`，以及整个 `outputs` 文件夹。不要把 `outputs/assets` 中的图片移到其他位置。
4. 点击页面底部的 **Commit changes**。
5. 进入仓库的 **Settings**。
6. 左侧点击 **Pages**。
7. 在 **Build and deployment** 中，将 **Source** 选择为 **Deploy from a branch**。
8. 在 **Branch** 中选择 `main`，文件夹选择 `/ (root)`。
9. 点击 **Save**。
10. 等待 GitHub Pages 显示发布地址，通常是：

```text
https://你的用户名.github.io/chucheng-jincheng/
```

把这个网址发给朋友，他们就可以直接打开游玩。

## 本地游玩

直接打开 `index.html`，或打开 `outputs/chucheng-jincheng.html`。

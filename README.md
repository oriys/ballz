# Ballz Web (Horizontal)

Canvas 弹射小游戏的横版网页版，支持瞄准拖拽、砖块/光球机制、加速快进、全屏切换。

## 运行

- 本地直接打开 `index.html` 即可游玩；或在根目录启动本地服务器：
  ```bash
  python3 -m http.server 8000
  ```
  然后浏览器访问 `http://localhost:8000`。

## 发布到 GitHub

1) 初始化并提交：
```bash
git init
git add .
git commit -m "chore: add ballz web"
```

2) 创建远程仓库（如 `ballz-web`），并推送：
```bash
git remote add origin git@github.com:<你的用户名>/ballz-web.git
git branch -M main
git push -u origin main
```

3) 开启 GitHub Pages：
- 在 GitHub 仓库 Settings -> Pages，Source 选择 `Deploy from a branch`，分支选择 `main`，目录选 `/(root)`，保存。
- 片刻后会获得一个公开 URL（如 `https://<用户名>.github.io/ballz-web/`），直接访问即可试玩。

## 控制

- 鼠标拖动瞄准，松手依次发射全部球。
- 空格或点击“加速 x3”按钮快进；“全屏”按钮可切换全屏。
- 回收首颗球的落点会作为下一回合的发射起点。

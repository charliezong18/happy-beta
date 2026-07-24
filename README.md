# happy-beta

Beta preview deploy target for [charliezong18/happy](https://github.com/charliezong18/happy). No source code lives here — the workflow checks out any branch from the fork and publishes it to https://charliezong18.github.io/happy-beta/. Production (`/happy/`) deploys from the fork repo and is never touched by this.

本仓库是 [charliezong18/happy](https://github.com/charliezong18/happy) 的 beta 预览部署目标，不含源码——workflow 从 fork checkout 任意分支，发布到 https://charliezong18.github.io/happy-beta/ 。正式版（`/happy/`）由 fork 仓库自己部署，与此互不影响。

## 用法 / Usage

    gh workflow run deploy-beta.yml -R charliezong18/happy-beta -f ref=<branch>

Or from a browser: **Actions → Deploy beta preview → Run workflow**, pick the branch.

# 中文上传步骤（仅公开版仓库）

以下步骤用于把当前 `public_release` 目录上传到你的 GitHub 仓库。

## 1. 进入目录

```powershell
cd <你的项目路径>\public_release
```

## 2. 初始化并提交（如已初始化可跳过前两条）

```powershell
git init
git checkout -b main
git add .
git commit -m "docs: 公开版项目说明"
```

## 3. 绑定远程仓库

```powershell
git remote add origin <你的GitHub仓库地址>
```

如果之前已经绑定过远程地址，改用：

```powershell
git remote set-url origin <你的GitHub仓库地址>
```

## 4. 推送到 GitHub

```powershell
git push -u origin main
```

如果远程分支需要覆盖（例如你重写了公开历史），使用：

```powershell
git push -f origin main
```

## 5. 上传后检查

```powershell
git remote -v
git branch --show-current
git log --oneline -n 3
```

打开 GitHub 仓库页面，确认：

- 显示的是公开版文档文件（README、docs）
- 不包含业务核心源码与敏感数据

# GitHub Pages 部署指南

## 步骤 1：创建 GitHub 仓库

1. 访问 https://github.com/new
2. 仓库名称填写：`sports-commentary-showcase`
3. 选择 **Public**（公开）
4. 点击 **Create repository**

## 步骤 2：获取 Personal Access Token

1. 访问 https://github.com/settings/tokens
2. 点击 **Generate new token (classic)**
3. 勾选 `repo` 权限
4. 点击 **Generate token**
5. **复制生成的 token**（只显示一次）

## 步骤 3：推送代码到 GitHub

在终端中执行以下命令（将 `YOUR_TOKEN` 替换为您的 token）：

```bash
cd "C:\Users\ygc66\AppData\Roaming\TRAE SOLO CN\ModularData\ai-agent\work-mode-projects\6a3942259efcd9fe68996558\sports-commentary-showcase"

# 设置远程仓库（使用 token 认证）
git remote add origin https://YOUR_TOKEN@github.com/ygc66/sports-commentary-showcase.git

# 推送代码
git push -u origin main
```

## 步骤 4：启用 GitHub Pages

1. 访问您的仓库页面：`https://github.com/ygc66/sports-commentary-showcase`
2. 点击 **Settings**（设置）
3. 左侧菜单点击 **Pages**
4. **Source** 选择 **Deploy from a branch**
5. **Branch** 选择 **main**，文件夹选择 **/(root)**
6. 点击 **Save**

## 步骤 5：访问网站

等待 1-2 分钟后，访问：

```
https://ygc66.github.io/sports-commentary-showcase/sports-commentary-showcase.html
```

## 注意事项

- 视频文件较大（约 100MB+），首次推送可能需要一些时间
- GitHub Pages 有 1GB 存储限制
- 如果视频太大，可以考虑使用外部视频托管服务（如哔哩哔哩、YouTube）嵌入

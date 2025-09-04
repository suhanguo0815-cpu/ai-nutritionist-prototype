# 部署指南

## 🚀 快速部署到GitHub Pages

### 方法一：使用GitHub Pages（推荐）

1. **创建GitHub仓库**
   ```bash
   # 在GitHub上创建一个新的仓库，命名为 "ai-nutritionist-demo"
   ```

2. **初始化Git仓库**
   ```bash
   cd /Users/guotongxue/Desktop/1-会员产品
   git init
   git add .
   git commit -m "Initial commit: AI营养师小程序完整原型"
   ```

3. **推送到GitHub**
   ```bash
   git remote add origin https://github.com/你的用户名/ai-nutritionist-demo.git
   git branch -M main
   git push -u origin main
   ```

4. **启用GitHub Pages**
   - 进入GitHub仓库设置
   - 找到 "Pages" 选项
   - 选择 "Deploy from a branch"
   - 选择 "main" 分支和 "/ (root)" 文件夹
   - 点击 "Save"

5. **访问链接**
   - 主页面：`https://你的用户名.github.io/ai-nutritionist-demo/`
   - 小程序演示：`https://你的用户名.github.io/ai-nutritionist-demo/demo`
   - 简化版本：`https://你的用户名.github.io/ai-nutritionist-demo/simple`

### 方法二：使用Vercel（更简单）

1. **安装Vercel CLI**
   ```bash
   npm i -g vercel
   ```

2. **部署**
   ```bash
   cd /Users/guotongxue/Desktop/1-会员产品
   vercel
   ```

3. **按照提示操作**
   - 选择项目类型：Other
   - 确认项目设置
   - 等待部署完成

4. **访问链接**
   - Vercel会自动提供一个链接，如：`https://ai-nutritionist-demo.vercel.app`

## 📱 移动端测试

部署完成后，建议在以下设备上测试：
- iPhone Safari
- Android Chrome
- 桌面端 Chrome/Firefox/Safari

## 🔧 自定义域名（可选）

如果您有自己的域名，可以：
1. 在Vercel或GitHub Pages设置中添加自定义域名
2. 配置DNS记录指向部署平台
3. 启用HTTPS

## 📊 性能优化

项目已包含以下优化：
- ✅ 图片压缩
- ✅ CSS/JS压缩
- ✅ 缓存策略
- ✅ 响应式设计
- ✅ 现代浏览器兼容性

## 🆘 常见问题

**Q: 部署后页面显示异常？**
A: 检查控制台错误，确保所有资源路径正确

**Q: 移动端显示有问题？**
A: 检查viewport设置和响应式CSS

**Q: 如何更新内容？**
A: 修改文件后重新提交到GitHub，Vercel会自动重新部署

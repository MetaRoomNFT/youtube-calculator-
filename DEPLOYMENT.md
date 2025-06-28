# 部署指南

## 🚀 快速部署选项

### 1. GitHub Pages (推荐 - 免费)

**步骤：**
1. 在GitHub上创建新仓库
2. 推送代码到GitHub：
   ```bash
   git remote add origin https://github.com/你的用户名/youtube-calculator.git
   git branch -M main
   git push -u origin main
   ```
3. 进入仓库设置 → Pages
4. 选择"Deploy from a branch"
5. 选择"main"分支和"/ (root)"文件夹
6. 点击"Save"
7. 等待几分钟，访问生成的URL

**优点：** 完全免费，自动HTTPS，CDN加速

### 2. Netlify (推荐 - 免费)

**步骤：**
1. 访问 [netlify.com](https://netlify.com) 注册账户
2. 点击"New site from Git"
3. 连接GitHub账户
4. 选择您的仓库
5. 保持默认设置，点击"Deploy site"
6. 等待部署完成，获得URL

**优点：** 自动部署，免费SSL，全球CDN

### 3. Vercel (推荐 - 免费)

**步骤：**
1. 访问 [vercel.com](https://vercel.com) 注册账户
2. 点击"New Project"
3. 导入GitHub仓库
4. 保持默认设置，点击"Deploy"
5. 等待部署完成，获得URL

**优点：** 极速部署，自动HTTPS，边缘网络

### 4. 传统虚拟主机

**步骤：**
1. 购买虚拟主机服务
2. 通过FTP上传所有文件到根目录
3. 确保index.html在根目录
4. 访问您的域名

### 5. 云服务器 (VPS)

**步骤：**
1. 购买云服务器
2. 安装Nginx或Apache
3. 上传文件到web目录
4. 配置域名解析

## 🔧 本地开发

### 使用Python服务器
```bash
python3 -m http.server 8000
# 访问 http://localhost:8000
```

### 使用Node.js服务器
```bash
npx serve .
# 访问 http://localhost:3000
```

### 使用PHP服务器
```bash
php -S localhost:8000
# 访问 http://localhost:8000
```

## 📝 部署前检查清单

- [ ] 所有文件已提交到Git
- [ ] index.html在根目录
- [ ] 测试所有功能正常工作
- [ ] 检查移动端适配
- [ ] 验证多语言切换
- [ ] 测试AI功能

## 🔒 安全配置

项目已包含基本的安全头配置：
- X-Frame-Options: DENY
- X-XSS-Protection: 1; mode=block
- X-Content-Type-Options: nosniff
- Referrer-Policy: strict-origin-when-cross-origin

## 🌐 自定义域名

### GitHub Pages
1. 在仓库设置中添加自定义域名
2. 在DNS提供商处添加CNAME记录

### Netlify/Vercel
1. 在平台设置中添加自定义域名
2. 按照平台指引配置DNS

## 📊 性能优化

- 使用CDN加速
- 启用Gzip压缩
- 设置缓存策略
- 优化图片资源

## 🆘 常见问题

**Q: 部署后AI功能不工作？**
A: 检查Gemini API密钥是否正确配置

**Q: 移动端显示异常？**
A: 确保viewport meta标签正确设置

**Q: 多语言切换不生效？**
A: 检查localStorage是否可用

## 📞 技术支持

如遇到部署问题，请检查：
1. 浏览器控制台错误信息
2. 网络连接状态
3. API服务可用性
4. 文件路径正确性 
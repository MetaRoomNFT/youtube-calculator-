# YouTube 频道收益计算器

一个免费的YouTube频道广告收入估算工具，支持多语言，并提供AI驱动的频道增长建议。

## 功能特点

- 🎯 **精准估算**: 基于公开API数据或智能模型估算频道收入
- 🌍 **多语言支持**: 支持10种语言（中文、英文、日文、西班牙文、法文、阿拉伯文、俄文、葡萄牙文、韩文）
- 🤖 **AI增长建议**: 集成Gemini AI提供个性化频道增长策略
- 📊 **详细分析**: 提供月度和年度收入预估
- 📱 **响应式设计**: 完美适配桌面和移动设备
- 💾 **历史记录**: 保存AI建议历史，方便回顾

## 技术栈

- HTML5
- CSS3 (Tailwind CSS)
- JavaScript (ES6+)
- Google Gemini AI API
- YouTube Data API (通过第三方服务)

## 部署方式

### GitHub Pages (推荐)
1. 将此仓库推送到GitHub
2. 在仓库设置中启用GitHub Pages
3. 选择main分支作为源
4. 访问生成的URL即可使用

### Netlify
1. 注册Netlify账户
2. 连接GitHub仓库
3. 自动部署完成

### Vercel
1. 注册Vercel账户
2. 导入GitHub仓库
3. 自动部署完成

## 本地开发

由于这是一个静态网站，您可以直接在浏览器中打开`index.html`文件，或者使用本地服务器：

```bash
# 使用Python
python -m http.server 8000

# 使用Node.js
npx serve .

# 使用PHP
php -S localhost:8000
```

## 使用说明

1. 输入YouTube频道URL（支持@用户名、频道ID等格式）
2. 点击"计算器"按钮获取收入估算
3. 点击"获取AI增长策略"获取个性化建议
4. 查看历史建议记录

## 注意事项

- 收入估算基于公开数据和行业模型，仅供参考
- 实际收入受多种因素影响，可能与估算结果有差异
- AI建议需要网络连接才能正常工作

## 许可证

MIT License 
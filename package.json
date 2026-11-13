const express = require('express');
const app = express();

const PORT = process.env.PORT || 3000;

// 直接使用当前目录作为静态文件目录
app.use(express.static(__dirname, { extensions: ['html'] }));

// 健康检查接口（Render 部署用）
app.get('/api/health', (req, res) => {
  res.send('OK');
});

app.listen(PORT, '0.0.0.0', () => {
  console.log(`Server is running on port ${PORT}`);
});

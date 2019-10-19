# Express

## 简单代码示例

```javascript
const express = require('express');
const app = express();
app.use('', (req, res, next) => {
    res.json({
        title: "Hello World"
    });
})
app.listen(3000, () => {
    console.log("Server is running on port 3000.");
});
```


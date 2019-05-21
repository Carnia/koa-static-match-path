
# 将静态资源映射到指定路由的中间件

## 依赖koa

### usage：

```js
/**
 * 中间件：
 * 将静态资源映射到指定路由
 * @param {*} customizePath 本地资源所在绝对路径
 * @param {string} [customizeStaticPath="static"] 路由名
 * @returns function
 */
const handleStatic = require('koa-static-path')

// 使用字符串
app.use(handleStatic(path.join(__dirname,'./public/'),'public'))

// 使用数组多映射
app.use(handleStatic(path.join(__dirname,'./static'),['static','source'])
```
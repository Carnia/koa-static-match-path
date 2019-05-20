###将静态资源映射到指定路由
usage：
```

/**
 * 中间件：
 * 将静态资源映射到指定路由
 * @param {*} customizePath 本地资源所在绝对路径
 * @param {string} [customizeStaticPath="static"] 路由名
 * @returns function
 */
const handleStatic = require('koa-static-path')
app.use(handleStatic(path.join(__dirname,'./public/'),'public'))
```
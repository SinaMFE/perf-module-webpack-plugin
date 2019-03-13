# perf-module-webpack-plugin


<h2 align="center">Scope</h2>

the plugin  computing time of all the modules bundled by webpack,and show the list of the top N modules who cost self execting.

it runs with dev server for it   injects code at runtime  will useless in prod; 

<h2 align="center">Install</h2>

```bash
npm i perf-module-webpack-plugin --save 
```

<h2 align="center"><a href="#">Usage</a></h2>

**webpack.dev.conf**

```js
const perfModuleWebpackPlugin =require("perf-module-webpack-plugin");
module.exports = {
  plugins:[
    new perfModuleWebpackPlugin({
        url:"http://exp.smfe.sina.cn/service/addPerf"// report server(post、cors),defalut null
      })
  ]
}
```

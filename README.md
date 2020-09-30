<!-- @format -->

# umi-plugin-dynamic-theme

> umi-plugin-antd-theme 的 fork 版本

[![NPM version](https://img.shields.io/npm/v/umi-plugin-dynamic-theme.svg?style=flat)](https://npmjs.org/package/umi-plugin-dynamic-theme) [![NPM downloads](http://img.shields.io/npm/dm/umi-plugin-dynamic-theme.svg?style=flat)](https://npmjs.org/package/umi-plugin-dynamic-theme)

## Usage

Configure in `config/theme.config.json`,

```json
{
  "theme": [
    {
      "theme": "dark",
      "fileName": "dark.css"
    },
    {
      "fileName": "mingQing.css",
      "modifyVars": {
        "@primary-color": "#13C2C2"
      }
    }
  ],
  // 是否压缩css
  "min": true,
  // css module
  "isModule": true,
  // 忽略 antd 的依赖
  "ignoreAntd": false,
  // 忽略 pro-layout
  "ignoreProLayout": false,
  // 不使用缓存
  "cache": true
}
```

or configure in `config/theme.config.js`,

```javascript
module.exports = {
  theme: [
    {
      theme: "dark",
      fileName: "dark.css",
    },
    {
      fileName: "mingQing.css",
      modifyVars: {
        "@primary-color": "#13C2C2",
      },
    },
  ],
  // 是否压缩css
  min: true,
  // css module
  isModule: true,
  // 忽略 antd 的依赖
  ignoreAntd: false,
  // 忽略 pro-layout
  ignoreProLayout: false,
  // 不使用缓存
  cache: true,
};
```

you can get config in `window.umi_plugin_ant_themeVar`

## LICENSE

MIT

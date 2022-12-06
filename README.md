# 代码规范配置

## prittier
https://prettier.io/docs/en/options.html#single-attribute-per-line

常用配置：
```json
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": false,
  "singleQuote": true,
  "endOfLine": "lf",
  "singleAttributePerLine": true,
  "vueIndentScriptAndStyle": true
}
```

## vuter
https://vuejs.github.io/vetur/guide/formatting.html#settings

常见问题：
1. 标签属性是否换行
默认强制换行：可设置为auto，跟prittier保持一致，也可将singleAttributePerLine设置为true
https://github.com/vuejs/vetur/blob/master/server/src/modes/template/services/htmlFormat.ts

常用配置：
```json
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": false,
  "singleQuote": true,
  "endOfLine": "lf",
  "singleAttributePerLine": true
}
```

关于vetur配置与prittier冲突，只需要将两者配置保持一致即可，prittier官网都有对应的配置可以与vetur保持一致

2. 标签与内容格式化时，内容应是单独一行
开启prittier:
 htmlWhitespaceSensitivity: true


vue模板中的配置
https://github.com/beautify-web/js-beautify
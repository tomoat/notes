# 在subl中使用正则表达式

使用一些简单的方法快速替换和修改subl中的文档内容

在subl中使用

## 简单的正则 (用于查找)

* `^` 表示开始
* `$` 表示结束
* `.*`　表示任意
* `\w` 表示数字和字母　`[0-9a-ZA-Z]`
* `\d` 表示数字　相当于　`[0-9]`
*　`＼　`　空格　特殊字符类似　`\|[]{}().` 等需要使用`\\`来转义
* `[]` 表示范围
* `{min,max}` 表示数量min,max都可以省略,　比如　`\d{1,}` 表示最少１个数字
* `()` 表示查找

用于替换`()`的范围使用 `\1` `\2` ... 

* 添加段落   ^(.*)$  替换为  <p>\1</p>
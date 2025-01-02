
## 背景与目标

让我们钻研一下正则表达式，这次先关注数字。
更确切地说，我们将学习如何处理你的应用程序中的电话号码。

## 详细说明

编写一个`french_phone_number?`方法，它以一个字符串作为参数，并返回一个布林值（boolean），当电话号码为有效的法国电话号码时为`true`:

- 当它以一个`0`开头，并含有10位数字时，则是有效的。第二位数字不能是0.
- 当它以`+33`开头，并含有11位数字时，也是有效的。并且紧跟在`+33`之后的数字不能是0.

该方法应该忽略数字之间的空格和划线。

```ruby
french_phone_number?("0665363636")
#=> true

french_phone_number?("06 65 36 36 36")
#=> true

french_phone_number?("01 36 65 36 65")
#=> true

french_phone_number?("06 65 36 36")
#=> false
```

## 进一步的建议

这里有一个很棒的资源，可以在你开始写代码之前测试一下你的regex：
[Rubular](http://rubular.com/)
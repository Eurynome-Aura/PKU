类型转变

| 函数                                                         | 描述                                                |
| :----------------------------------------------------------- | :-------------------------------------------------- |
| [int(x [,base\])](https://www.runoob.com/python/python-func-int.html)   x -- 字符串或数字，base -- 进制数，默认十进制 | 将x转换为一个整数                                   |
| [long(x [,base\] )](https://www.runoob.com/python/python-func-long.html) | 将x转换为一个长整数                                 |
| [float(x)](https://www.runoob.com/python/python-func-float.html) | 将x转换到一个浮点数                                 |
| [complex(real [,imag\])](https://www.runoob.com/python/python-func-complex.html) | 创建一个复数                                        |
| [str(x)](https://www.runoob.com/python/python-func-str.html) | 将对象 x 转换为字符串                               |
| [repr(x)](https://www.runoob.com/python/python-func-repr.html) | 将对象 x 转换为表达式字符串                         |
| [eval(str)](https://www.runoob.com/python/python-func-eval.html) | 用来计算在字符串中的有效Python表达式,并返回一个对象 |
| [tuple(s)](https://www.runoob.com/python/att-tuple-tuple.html) | 将序列 s 转换为一个元组                             |
| [list(s)](https://www.runoob.com/python/att-list-list.html)  | 将序列 s 转换为一个列表                             |
| [set(s)](https://www.runoob.com/python/python-func-set.html) | 转换为可变集合                                      |
| [dict(d)](https://www.runoob.com/python/python-func-dict.html) | 创建一个字典。d 必须是一个序列 (key,value)元组。    |
| [frozenset(s)](https://www.runoob.com/python/python-func-frozenset.html) | 转换为不可变集合                                    |
| [chr(x)](https://www.runoob.com/python/python-func-chr.html) | 将一个整数转换为一个字符                            |
| [unichr(x)](https://www.runoob.com/python/python-func-unichr.html) | 将一个整数转换为Unicode字符                         |
| [ord(x)](https://www.runoob.com/python/python-func-ord.html) | 将一个字符转换为它的整数值                          |
| [hex(x)](https://www.runoob.com/python/python-func-hex.html) | 将一个整数转换为一个十六进制字符串                  |
| [oct(x)](https://www.runoob.com/python/python-func-oct.html) | 将一个整数转换为一个八进制字符串                    |

```python
>>> int('12',16)        # 如果是带参数base的话，12要以字符串的形式进行输入，12 为 16进制
18
```

运算符

| +    | 加 - 两个对象相加                               | a + b 输出结果 30                                  |
| ---- | ----------------------------------------------- | -------------------------------------------------- |
| -    | 减 - 得到负数或是一个数减去另一个数             | a - b 输出结果 -10                                 |
| *    | 乘 - 两个数相乘或是返回一个被重复若干次的字符串 | a * b 输出结果 200                                 |
| /    | 除 - x除以y                                     | b / a 输出结果 2                                   |
| %    | 取模 - 返回除法的余数                           | b % a 输出结果 0                                   |
| **   | 幂 - 返回x的y次幂                               | a**b 为10的20次方， 输出结果 100000000000000000000 |
| //   | 取整除 - 返回商的整数部分（**向下取整**）       | `>>> 9//2 4 >>> -9//2 -5`                          |

| 运算符 | 描述                                                         | 实例                  |
| :----- | :----------------------------------------------------------- | :-------------------- |
| ==     | 等于 - 比较对象是否相等                                      | (a == b) 返回 False。 |
| !=     | 不等于 - 比较两个对象是否不相等                              | (a != b) 返回 True。  |
| >      | 大于 - 返回x是否大于y                                        | (a > b) 返回 False。  |
| <      | 小于 - 返回x是否小于y。所有比较运算符返回1表示真，返回0表示假。这分别与特殊的变量 True 和 False 等价。 | (a < b) 返回 True。   |
| >=     | 大于等于 - 返回x是否大于等于y。                              | (a >= b) 返回 False。 |
| <=     | 小于等于 - 返回x是否小于等于y。                              | (a <= b) 返回 True。  |

| 运算符 | 描述                                                         | 实例                                                         |
| :----- | :----------------------------------------------------------- | :----------------------------------------------------------- |
| &      | 按位与运算符：参与运算的两个值,如果两个相应位都为1,则该位的结果为1,否则为0 | (a & b) 输出结果 12 ，二进制解释： 0000 1100                 |
| \|     | 按位或运算符：只要对应的二个二进位有一个为1时，结果位就为1。 | (a \| b) 输出结果 61 ，二进制解释： 0011 1101                |
| ^      | 按位异或运算符：当两对应的二进位相异时，结果为1              | (a ^ b) 输出结果 49 ，二进制解释： 0011 0001                 |
| ~      | 按位取反运算符：对数据的每个二进制位取反,即把1变为0,把0变为1 。**~x** 类似于 **-x-1** | (~a ) 输出结果 -61 ，二进制解释： 1100 0011，在一个有符号二进制数的补码形式。 |
| <<     | 左移动运算符：运算数的各二进位全部左移若干位，由 **<<** 右边的数字指定了移动的位数，高位丢弃，低位补0。 | a << 2 输出结果 240 ，二进制解释： 1111 0000                 |
| >>     | 右移动运算符：把">>"左边的运算数的各二进位全部右移若干位，**>>** 右边的数字指定了移动的位数 | a >> 2 输出结果 15 ，二进制解释： 0000 1111                  |

| 运算符 | 逻辑表达式 | 描述                                                         | 实例                    |
| :----- | :--------- | :----------------------------------------------------------- | :---------------------- |
| and    | x and y    | 布尔"与" - 如果 x 为 False，x and y 返回 False，否则它返回 y 的计算值。 | (a and b) 返回 20。     |
| or     | x or y     | 布尔"或" - 如果 x 是非 0，它返回 x 的计算值，否则它返回 y 的计算值。 | (a or b) 返回 10。      |
| not    | not x      | 布尔"非" - 如果 x 为 True，返回 False 。如果 x 为 False，它返回 True。 | not(a and b) 返回 False |

| 运算符 | 描述                                                    | 实例                                              |
| :----- | :------------------------------------------------------ | :------------------------------------------------ |
| in     | 如果在指定的序列中找到值返回 True，否则返回 False。     | x 在 y 序列中 , 如果 x 在 y 序列中返回 True。     |
| not in | 如果在指定的序列中没有找到值返回 True，否则返回 False。 | x 不在 y 序列中 , 如果 x 不在 y 序列中返回 True。 |

| 运算符 | 描述                                        | 实例                                                         |
| :----- | :------------------------------------------ | :----------------------------------------------------------- |
| is     | is 是判断两个标识符是不是引用自一个对象     | **x is y**, 类似 **id(x) == id(y)** , 如果引用的是同一个对象则返回 True，否则返回 False |
| is not | is not 是判断两个标识符是不是引用自不同对象 | **x is not y** ， 类似 **id(a) != id(b)**。如果引用的不是同一个对象则返回结果 True，否则返回 False。 |

以下表格列出了从最高到最低优先级的所有运算符：

| 运算符                   | 描述                                                   |
| :----------------------- | :----------------------------------------------------- |
| **                       | 指数 (最高优先级)                                      |
| ~ + -                    | 按位翻转, 一元加号和减号 (最后两个的方法名为 +@ 和 -@) |
| * / % //                 | 乘，除，取模和取整除                                   |
| + -                      | 加法减法                                               |
| >> <<                    | 右移，左移运算符                                       |
| &                        | 位 'AND'                                               |
| ^ \|                     | 位运算符                                               |
| <= < > >=                | 比较运算符                                             |
| <> == !=                 | 等于运算符                                             |
| = %= /= //= -= += *= **= | 赋值运算符                                             |
| is is not                | 身份运算符                                             |
| in not in                | 成员运算符                                             |
| not and or               | 逻辑运算符                                             |

```python
>>> import math
>>> dir(math)
['__doc__', '__file__', '__loader__', '__name__', '__package__', '__spec__', 'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'ceil', 'copysign', 'cos', 'cosh', 'degrees', 'e', 'erf', 'erfc', 'exp', 'expm1', 'fabs', 'factorial', 'floor', 'fmod', 'frexp', 'fsum', 'gamma', 'gcd', 'hypot', 'inf', 'isclose', 'isfinite', 'isinf', 'isnan', 'ldexp', 'lgamma', 'log', 'log10', 'log1p', 'log2', 'modf', 'nan', 'pi', 'pow', 'radians', 'sin', 'sinh', 'sqrt', 'tan', 'tanh', 'tau', 'trunc']
>>>math.sin?
>>>Signature: math.sin(x, /)
Docstring: Return the sine of x (measured in radians).
Type:      builtin_function_or_method
```

| 函数                                                         | 返回值 ( 描述 )                                              |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [abs(x)](https://www.runoob.com/python/func-number-abs.html) | 返回数字的绝对值，如abs(-10) 返回 10                         |
| [ceil(x)](https://www.runoob.com/python/func-number-ceil.html) | 返回数字的上入整数，如math.ceil(4.1) 返回 5                  |
| [cmp(x, y)](https://www.runoob.com/python/func-number-cmp.html) | 如果 x < y 返回 -1, 如果 x == y 返回 0, 如果 x > y 返回 1    |
| [exp(x)](https://www.runoob.com/python/func-number-exp.html) | 返回e的x次幂(ex),如math.exp(1) 返回2.718281828459045         |
| [fabs(x)](https://www.runoob.com/python/func-number-fabs.html) | 以浮点数形式返回数字的绝对值，如math.fabs(-10) 返回10.0      |
| [floor(x)](https://www.runoob.com/python/func-number-floor.html) | 返回数字的下舍整数，如math.floor(4.9)返回 4                  |
| [log(x)](https://www.runoob.com/python/func-number-log.html) | 如math.log(math.e)返回1.0,math.log(100,10)返回2.0            |
| [log10(x)](https://www.runoob.com/python/func-number-log10.html) | 返回以10为基数的x的对数，如math.log10(100)返回 2.0           |
| [max(x1, x2,...)](https://www.runoob.com/python/func-number-max.html) | 返回给定参数的最大值，参数可以为序列。                       |
| [min(x1, x2,...)](https://www.runoob.com/python/func-number-min.html) | 返回给定参数的最小值，参数可以为序列。                       |
| [modf(x)](https://www.runoob.com/python/func-number-modf.html) | 返回x的整数部分与小数部分，两部分的数值符号与x相同，整数部分以浮点型表示。 |
| [pow(x, y)](https://www.runoob.com/python/func-number-pow.html) | x**y 运算后的值。                                            |
| [round(x [,n\])](https://www.runoob.com/python/func-number-round.html) | 返回浮点数x的四舍五入值，如给出n值，则代表舍入到小数点后的位数。 |
| [sqrt(x)](https://www.runoob.com/python/func-number-sqrt.html) | 返回数字x的平方根                                            |

字符串

| 操作符 | 描述                                                         | 实例                                 |
| :----- | :----------------------------------------------------------- | :----------------------------------- |
| +      | 字符串连接                                                   | >>>a + b 'HelloPython'               |
| *      | 重复输出字符串                                               | >>>a * 2 'HelloHello'                |
| []     | 通过索引获取字符串中字符                                     | >>>a[1] 'e'                          |
| [ : ]  | 截取字符串中的一部分                                         | >>>a[1:4] 'ell'                      |
| in     | 成员运算符 - 如果字符串中包含给定的字符返回 True             | >>>"H" in a True                     |
| not in | 成员运算符 - 如果字符串中不包含给定的字符返回 True           | >>>"M" not in a True                 |
| r/R    | 原始字符串 - 原始字符串：所有的字符串都是直接按照字面的意思来使用，没有转义特殊或不能打印的字符。 原始字符串除在字符串的第一个引号前加上字母"r"（可以大小写）以外，与普通字符串有着几乎完全相同的语法。 | >>>print r'\n' \n >>> print R'\n' \n |
| %      | 格式字符串                                                   | 请看下一章节                         |

```python
print "My name is %s and weight is %d kg!" % ('Zara', 21)
My name is Zara and weight is 21 kg!
```

格式化操作符辅助指令:

| 符  号 | 描述                                 |
| :----- | :----------------------------------- |
| %c     | 格式化字符及其ASCII码                |
| %s     | 格式化字符串                         |
| %d     | 格式化整数                           |
| %u     | 格式化无符号整型                     |
| %o     | 格式化无符号八进制数                 |
| %x     | 格式化无符号十六进制数               |
| %X     | 格式化无符号十六进制数（大写）       |
| %f     | 格式化浮点数字，可指定小数点后的精度 |
| %e     | 用科学计数法格式化浮点数             |
| %E     | 作用同%e，用科学计数法格式化浮点数   |
| %g     | %f和%e的简写                         |
| %G     | %F 和 %E 的简写                      |
| %p     | 用十六进制数格式化变量的地址         |

| 符号  | 功能                                                         |
| :---- | :----------------------------------------------------------- |
| *     | 定义宽度或者小数点精度                                       |
| -     | 用做左对齐                                                   |
| +     | 在正数前面显示加号( + )                                      |
| <sp>  | 在正数前面显示空格                                           |
| #     | 在八进制数前面显示零('0')，在十六进制前面显示'0x'或者'0X'(取决于用的是'x'还是'X') |
| 0     | 显示的数字前面填充'0'而不是默认的空格                        |
| %     | '%%'输出一个单一的'%'                                        |
| (var) | 映射变量(字典参数)                                           |
| m.n.  | m 是显示的最小总宽度,n 是小数点后的位数(如果可用的话)        |

## Python 的字符串内建函数

询问操作：str.lower?

| **方法**                                                     | **描述**                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| [string.capitalize()](https://www.runoob.com/python/att-string-capitalize.html) | 把字符串的第一个字符大写                                     |
| [string.center(width)](https://www.runoob.com/python/att-string-center.html) | 返回一个原字符串居中,并使用空格填充至长度 width 的新字符串   |
| **[string.count(str, beg=0, end=len(string))](https://www.runoob.com/python/att-string-count.html)** | 返回 str 在 string 里面出现的次数，如果 beg 或者 end 指定则返回指定范围内 str 出现的次数 |
| [string.decode(encoding='UTF-8', errors='strict')](https://www.runoob.com/python/att-string-decode.html) | 以 encoding 指定的编码格式解码 string，如果出错默认报一个 ValueError 的 异 常 ， 除非 errors 指 定 的 是 'ignore' 或 者'replace' |
| [string.encode(encoding='UTF-8', errors='strict')](https://www.runoob.com/python/att-string-encode.html) | 以 encoding 指定的编码格式编码 string，如果出错默认报一个ValueError 的异常，除非 errors 指定的是'ignore'或者'replace' |
| **[string.endswith(obj, beg=0, end=len(string))](https://www.runoob.com/python/att-string-endswith.html)** | 检查字符串是否以 obj 结束，如果beg 或者 end 指定则检查指定的范围内是否以 obj 结束，如果是，返回 True,否则返回 False. |
| [string.expandtabs(tabsize=8)](https://www.runoob.com/python/att-string-expandtabs.html) | 把字符串 string 中的 tab 符号转为空格，tab 符号默认的空格数是 8。 |
| **[string.find(str, beg=0, end=len(string))](https://www.runoob.com/python/att-string-find.html)** | 检测 str 是否包含在 string 中，如果 beg 和 end 指定范围，则检查是否包含在指定范围内，如果是返回开始的索引值，否则返回-1 |
| **[string.format()](https://www.runoob.com/python/att-string-format.html)** | 格式化字符串                                                 |
| **[string.index(str, beg=0, end=len(string))](https://www.runoob.com/python/att-string-index.html)** | 跟find()方法一样，只不过如果str不在 string中会报一个异常.    |
| [string.isalnum()](https://www.runoob.com/python/att-string-isalnum.html) | 如果 string 至少有一个字符并且所有字符都是字母或数字则返回 True,否则返回 False |
| [string.isalpha()](https://www.runoob.com/python/att-string-isalpha.html) | 如果 string 至少有一个字符并且所有字符都是字母则返回 True,否则返回 False |
| [string.isdecimal()](https://www.runoob.com/python/att-string-isdecimal.html) | 如果 string 只包含十进制数字则返回 True 否则返回 False.      |
| [string.isdigit()](https://www.runoob.com/python/att-string-isdigit.html) | 如果 string 只包含数字则返回 True 否则返回 False.            |
| [string.islower()](https://www.runoob.com/python/att-string-islower.html) | 如果 string 中包含至少一个区分大小写的字符，并且所有这些(区分大小写的)字符都是小写，则返回 True，否则返回 False |
| [string.isnumeric()](https://www.runoob.com/python/att-string-isnumeric.html) | 如果 string 中只包含数字字符，则返回 True，否则返回 False    |
| [string.isspace()](https://www.runoob.com/python/att-string-isspace.html) | 如果 string 中只包含空格，则返回 True，否则返回 False.       |
| [string.istitle()](https://www.runoob.com/python/att-string-istitle.html) | 如果 string 是标题化的(见 title())则返回 True，否则返回 False |
| [string.isupper()](https://www.runoob.com/python/att-string-isupper.html) | 如果 string 中包含至少一个区分大小写的字符，并且所有这些(区分大小写的)字符都是大写，则返回 True，否则返回 False |
| **[string.join(seq)](https://www.runoob.com/python/att-string-join.html)** | 以 string 作为分隔符，将 seq 中所有的元素(的字符串表示)合并为一个新的字符串 |
| [string.ljust(width)](https://www.runoob.com/python/att-string-ljust.html) | 返回一个原字符串左对齐,并使用空格填充至长度 width 的新字符串 |
| [string.lower()](https://www.runoob.com/python/att-string-lower.html) | 转换 string 中所有大写字符为小写.                            |
| [string.lstrip()](https://www.runoob.com/python/att-string-lstrip.html) | 截掉 string 左边的空格                                       |
| [string.maketrans(intab, outtab)](https://www.runoob.com/python/att-string-maketrans.html) | maketrans() 方法用于创建字符映射的转换表，对于接受两个参数的最简单的调用方式，第一个参数是字符串，表示需要转换的字符，第二个参数也是字符串表示转换的目标。 |
| [max(str)](https://www.runoob.com/python/att-string-max.html) | 返回字符串 *str* 中最大的字母。                              |
| [min(str)](https://www.runoob.com/python/att-string-min.html) | 返回字符串 *str* 中最小的字母。                              |
| **[string.partition(str)](https://www.runoob.com/python/att-string-partition.html)** | 有点像 find()和 split()的结合体,从 str 出现的第一个位置起,把 字 符 串 string 分 成 一 个 3 元 素 的 元 组 (string_pre_str,str,string_post_str),如果 string 中不包含str 则 string_pre_str == string. |
| **[string.replace(str1, str2, num=string.count(str1))](https://www.runoob.com/python/att-string-replace.html)** | 把 string 中的 str1 替换成 str2,如果 num 指定，则替换不超过 num 次. |
| [string.rfind(str, beg=0,end=len(string) )](https://www.runoob.com/python/att-string-rfind.html) | 类似于 find() 函数，返回字符串最后一次出现的位置，如果没有匹配项则返回 -1。 |
| [string.rindex( str, beg=0,end=len(string))](https://www.runoob.com/python/att-string-rindex.html) | 类似于 index()，不过是返回最后一个匹配到的子字符串的索引号。 |
| [string.rjust(width)](https://www.runoob.com/python/att-string-rjust.html) | 返回一个原字符串右对齐,并使用空格填充至长度 width 的新字符串 |
| [string.rpartition(str)](https://www.runoob.com/python/att-string-rpartition.html) | 类似于 partition()函数,不过是从右边开始查找                  |
| [string.rstrip()](https://www.runoob.com/python/att-string-rstrip.html) | 删除 string 字符串末尾的空格.                                |
| **[string.split(str="", num=string.count(str))](https://www.runoob.com/python/att-string-split.html)** | 以 str 为分隔符切片 string，如果 num 有指定值，则仅分隔 **num+1** 个子字符串 |
| [string.splitlines([keepends\])](https://www.runoob.com/python/att-string-splitlines.html) | 按照行('\r', '\r\n', '\n')分隔，返回一个包含各行作为元素的列表，如果参数 keepends 为 False，不包含换行符，如果为 True，则保留换行符。 |
| [string.startswith(obj, beg=0,end=len(string))](https://www.runoob.com/python/att-string-startswith.html) | 检查字符串是否是以 obj 开头，是则返回 True，否则返回 False。如果beg 和 end 指定值，则在指定范围内检查. |
| **[string.strip([obj\])](https://www.runoob.com/python/att-string-strip.html)** | 在 string 上执行 lstrip()和 rstrip()                         |
| [string.swapcase()](https://www.runoob.com/python/att-string-swapcase.html) | 翻转 string 中的大小写                                       |
| [string.title()](https://www.runoob.com/python/att-string-title.html) | 返回"标题化"的 string,就是说所有单词都是以大写开始，其余字母均为小写(见 istitle()) |
| **[string.translate(str, del="")](https://www.runoob.com/python/att-string-translate.html)** | 根据 str 给出的表(包含 256 个字符)转换 string 的字符,要过滤掉的字符放到 del 参数中 |
| [string.upper()](https://www.runoob.com/python/att-string-upper.html) | 转换 string 中的小写字母为大写                               |
| [string.zfill(width)](https://www.runoob.com/python/att-string-zfill.html) | 返回长度为 width 的字符串，原字符串 string 右对齐，前面填充0 |

```python
symbol = "-";
seq = ("a", "b", "c"); # 字符串序列
print symbol.join( seq );
```





列表

| Python 表达式                | 结果                         | 描述                 |
| :--------------------------- | :--------------------------- | :------------------- |
| len([1, 2, 3])               | 3                            | 长度                 |
| [1, 2, 3] + [4, 5, 6]        | [1, 2, 3, 4, 5, 6]           | 组合                 |
| ['Hi!'] * 4                  | ['Hi!', 'Hi!', 'Hi!', 'Hi!'] | 重复                 |
| 3 in [1, 2, 3]               | True                         | 元素是否存在于列表中 |
| for x in [1, 2, 3]: print x, | 1 2 3                        | 迭代                 |

| 序号 | 函数                                                         |
| :--- | :----------------------------------------------------------- |
| 1    | [cmp(list1, list2)](https://www.runoob.com/python/att-list-cmp.html) 比较两个列表的元素 |
| 2    | [len(list)](https://www.runoob.com/python/att-list-len.html) 列表元素个数 |
| 3    | [max(list)](https://www.runoob.com/python/att-list-max.html) 返回列表元素最大值 |
| 4    | [min(list)](https://www.runoob.com/python/att-list-min.html) 返回列表元素最小值 |
| 5    | [list(seq)](https://www.runoob.com/python/att-list-list.html) 将元组转换为列表 |

| 序号 | 方法                                                         |
| :--- | :----------------------------------------------------------- |
| 1    | [list.append(obj)](https://www.runoob.com/python/att-list-append.html) 在列表末尾添加新的对象 |
| 2    | [list.count(obj)](https://www.runoob.com/python/att-list-count.html) 统计某个元素在列表中出现的次数 |
| 3    | [list.extend(seq)](https://www.runoob.com/python/att-list-extend.html) 在列表末尾一次性追加另一个序列中的多个值（用新列表扩展原来的列表） |
| 4    | [list.index(obj)](https://www.runoob.com/python/att-list-index.html) 从列表中找出某个值第一个匹配项的索引位置 |
| 5    | [list.insert(index, obj)](https://www.runoob.com/python/att-list-insert.html) 将对象插入列表 |
| 6    | [list.pop([index=-1\])](https://www.runoob.com/python/att-list-pop.html) 移除列表中的一个元素（默认最后一个元素），并且返回该元素的值 |
| 7    | [list.remove(obj)](https://www.runoob.com/python/att-list-remove.html) 移除列表中某个值的第一个匹配项 |
| 8    | [list.reverse()](https://www.runoob.com/python/att-list-reverse.html) 反向列表中元素 |
| 9    | [list.sort(cmp=None, key=None, reverse=False)](https://www.runoob.com/python/att-list-sort.html) 对原列表进行排序 |

字典

```python
dict = {}
dict['one'] = "This is one"
dict[2] = "This is two"

tinydict = {'name': 'runoob','code':6734, 'dept': 'sales'}

print dict['one']          # 输出键为'one' 的值
print dict[2]              # 输出键为 2 的值
print tinydict             # 输出完整的字典
print tinydict.keys()      # 输出所有键
print tinydict.values()    # 输出所有值

This is one
This is two
{'dept': 'sales', 'code': 6734, 'name': 'runoob'}
['dept', 'code', 'name']
['sales', 6734, 'runoob']

>>>dict()                        # 创建空字典
{}
>>> dict(a='a', b='b', t='t')     # 传入关键字
{'a': 'a', 'b': 'b', 't': 't'}
>>> dict(zip(['one', 'two', 'three'], [1, 2, 3]))   # 映射函数方式来构造字典
{'three': 3, 'two': 2, 'one': 1} 
>>> dict([('one', 1), ('two', 2), ('three', 3)])    # 可迭代对象方式来构造字典
{'three': 3, 'two': 2, 'one': 1}
>>>
```

```python
d = {key1 : value1, key2 : value2 }

>>> tinydict = {'a': 1, 'b': 2, 'b': '3'}
>>> tinydict['b']
'3'

tinydict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}

tinydict['Age'] = 8 # 更新
tinydict['School'] = "RUNOOB" # 添加

tinydict = {'Name': 'Zara', 'Age': 7, 'Class': 'First'}
 
del tinydict['Name']  # 删除键是'Name'的条目
tinydict.clear()      # 清空字典所有条目
del tinydict          # 删除字典
```

| 序号 | 函数及描述                                                   |
| :--- | :----------------------------------------------------------- |
| 1    | [cmp(dict1, dict2)](https://www.runoob.com/python/att-dictionary-cmp.html) 比较两个字典元素。 |
| 2    | [len(dict)](https://www.runoob.com/python/att-dictionary-len.html) 计算字典元素个数，即键的总数。 |
| 3    | [str(dict)](https://www.runoob.com/python/att-dictionary-str.html) 输出字典可打印的字符串表示。 |
| 4    | [type(variable)](https://www.runoob.com/python/att-dictionary-type.html) 返回输入的变量类型，如果变量是字典就返回字典类型。 |

| 序号 | 函数及描述                                                   |
| :--- | :----------------------------------------------------------- |
| 1    | [dict.clear()](https://www.runoob.com/python/att-dictionary-clear.html) 删除字典内所有元素 |
| 2    | [dict.copy()](https://www.runoob.com/python/att-dictionary-copy.html) 返回一个字典的浅复制 |
| 3    | [dict.fromkeys(seq[, val\])](https://www.runoob.com/python/att-dictionary-fromkeys.html) 创建一个新字典，以序列 seq 中元素做字典的键，val 为字典所有键对应的初始值 |
| 4    | [dict.get(key, default=None)](https://www.runoob.com/python/att-dictionary-get.html) 返回指定键的值，如果值不在字典中返回default值 |
| 5    | [dict.has_key(key)](https://www.runoob.com/python/att-dictionary-has_key.html) 如果键在字典dict里返回true，否则返回false。Python3 不支持。 |
| 6    | [dict.items()](https://www.runoob.com/python/att-dictionary-items.html) 以列表返回可遍历的(键, 值) 元组数组 |
| 7    | [dict.keys()](https://www.runoob.com/python/att-dictionary-keys.html) 以列表返回一个字典所有的键 |
| 8    | [dict.setdefault(key, default=None)](https://www.runoob.com/python/att-dictionary-setdefault.html) 和get()类似, 但如果键不存在于字典中，将会添加键并将值设为default |
| 9    | [dict.update(dict2)](https://www.runoob.com/python/att-dictionary-update.html) 把字典dict2的键/值对更新到dict里 |
| 10   | [dict.values()](https://www.runoob.com/python/att-dictionary-values.html) 以列表返回字典中的所有值 |
| 11   | [pop(key[,default\])](https://www.runoob.com/python/python-att-dictionary-pop.html) 删除字典给定键 key 所对应的值，返回值为被删除的值。key值必须给出。 否则，返回default值。 |
| 12   | [popitem()](https://www.runoob.com/python/python-att-dictionary-popitem.html) 返回并删除字典中的最后一对键和值。 |

### 可更改(mutable)与不可更改(immutable)对象

在 python 中，strings, tuples, 和 numbers 是不可更改的对象，而 list,dict 等则是可以修改的对象。

- **不可变类型：**变量赋值 **a=5** 后再赋值 **a=10**，这里实际是新生成一个 int 值对象 10，再让 a 指向它，而 5 被丢弃，不是改变a的值，相当于新生成了a。
- **可变类型：**变量赋值 **la=[1,2,3,4]** 后再赋值 **la[2]=5** 则是将 list la 的第三个元素值更改，本身la没有动，只是其内部的一部分值被修改了。

python 函数的参数传递：

- **不可变类型：**类似 c++ 的值传递，如 整数、字符串、元组。如fun（a），传递的只是a的值，没有影响a对象本身。比如在 fun（a）内部修改 a 的值，只是修改另一个复制的对象，不会影响 a 本身。
- **可变类型：**类似 c++ 的引用传递，如 列表，字典。如 fun（la），则是将 la 真正的传过去，修改后fun外部的la也会受影响

```python
 def ChangeInt( a ):
    a = 10
 
b = 2
ChangeInt(b)
print b # 结果是 2
```

```python
def changeme( mylist ):
   "修改传入的列表"
   mylist.append([1,2,3,4])
   print "函数内取值: ", mylist
   return
 
# 调用changeme函数
mylist = [10,20,30]
changeme( mylist )
print "函数外取值: ", mylist

函数内取值:  [10, 20, 30, [1, 2, 3, 4]]
函数外取值:  [10, 20, 30, [1, 2, 3, 4]]
```

```python
def printinfo( name, age ):
   "打印任何传入的字符串"
   print "Name: ", name
   print "Age ", age
   return
printinfo( age=50, name="miki" )

def printinfo( name, age = 35 ):
   "打印任何传入的字符串"
   print "Name: ", name
   print "Age ", age
   return
printinfo( age=50, name="miki" )
printinfo( name="miki" )

def printinfo( arg1, *vartuple ):
   "打印任何传入的参数"
   print "输出: "
   print arg1
   for var in vartuple:
      print var
   return
printinfo( 10 )
printinfo( 70, 60, 50 )

sum = lambda arg1, arg2: arg1 + arg2
print "相加后的值为 : ", sum( 10, 20 )
print "相加后的值为 : ", sum( 20, 20 )
```

| 异常名称                  | 描述                                               |
| :------------------------ | :------------------------------------------------- |
|                           |                                                    |
| BaseException             | 所有异常的基类                                     |
| SystemExit                | 解释器请求退出                                     |
| KeyboardInterrupt         | 用户中断执行(通常是输入^C)                         |
| Exception                 | 常规错误的基类                                     |
| StopIteration             | 迭代器没有更多的值                                 |
| GeneratorExit             | 生成器(generator)发生异常来通知退出                |
| StandardError             | 所有的内建标准异常的基类                           |
| ArithmeticError           | 所有数值计算错误的基类                             |
| FloatingPointError        | 浮点计算错误                                       |
| OverflowError             | 数值运算超出最大限制                               |
| ZeroDivisionError         | 除(或取模)零 (所有数据类型)                        |
| AssertionError            | 断言语句失败                                       |
| AttributeError            | 对象没有这个属性                                   |
| EOFError                  | 没有内建输入,到达EOF 标记                          |
| EnvironmentError          | 操作系统错误的基类                                 |
| IOError                   | 输入/输出操作失败                                  |
| OSError                   | 操作系统错误                                       |
| WindowsError              | 系统调用失败                                       |
| ImportError               | 导入模块/对象失败                                  |
| LookupError               | 无效数据查询的基类                                 |
| IndexError                | 序列中没有此索引(index)                            |
| KeyError                  | 映射中没有这个键                                   |
| MemoryError               | 内存溢出错误(对于Python 解释器不是致命的)          |
| NameError                 | 未声明/初始化对象 (没有属性)                       |
| UnboundLocalError         | 访问未初始化的本地变量                             |
| ReferenceError            | 弱引用(Weak reference)试图访问已经垃圾回收了的对象 |
| RuntimeError              | 一般的运行时错误                                   |
| NotImplementedError       | 尚未实现的方法                                     |
| SyntaxError               | Python 语法错误                                    |
| IndentationError          | 缩进错误                                           |
| TabError                  | Tab 和空格混用                                     |
| SystemError               | 一般的解释器系统错误                               |
| TypeError                 | 对类型无效的操作                                   |
| ValueError                | 传入无效的参数                                     |
| UnicodeError              | Unicode 相关的错误                                 |
| UnicodeDecodeError        | Unicode 解码时的错误                               |
| UnicodeEncodeError        | Unicode 编码时错误                                 |
| UnicodeTranslateError     | Unicode 转换时错误                                 |
| Warning                   | 警告的基类                                         |
| DeprecationWarning        | 关于被弃用的特征的警告                             |
| FutureWarning             | 关于构造将来语义会有改变的警告                     |
| OverflowWarning           | 旧的关于自动提升为长整型(long)的警告               |
| PendingDeprecationWarning | 关于特性将会被废弃的警告                           |
| RuntimeWarning            | 可疑的运行时行为(runtime behavior)的警告           |
| SyntaxWarning             | 可疑的语法的警告                                   |
| UserWarning               | 用户代码生成的警告                                 |

```python
b="+".join(s)
print(b)

print("Cube = %d, Triple = (%d,%d,%d)"%(result[i][0],result[i][1]\
                                            ,result[i][2],result[i][3]))
for i in range(n):
    print(*c[i],sep=' ')
print("%.1f"%(value))
result = "{:.6f}".format(s[0])
print(result)

	maze.append(['.' for i in range(m+2)])
    for i in range(n):
        s=['.']+[j for j in input()]+['.']
        maze.append(s)
    maze.append(['.' for i in range(m+2)])
```

### 动规

##### 最长上升子序列

```python
import bisect
n = int(input())
*lis, = map(int, input().split())
dp = [1e9]*n
for i in lis:
    dp[bisect.bisect_left(dp, i)] = i
print(bisect.bisect_left(dp, 1e8))
```

##### 背包问题

![image-20231227152549929](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227152549929.png)

![image-20231227152648621](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227152648621.png)

### dfs

![image-20231227223054681](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227223054681.png)

![image-20231227223112978](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227223112978.png)

### bfs

![image-20231227223727865](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227223727865.png)

![image-20231227223739425](C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227223739425.png)





例题

排队

```python
# -*- coding: utf-8 -*-
"""
Created on Wed Sep 20 09:51:17 2023

@author: 40864
"""

sp = input().split()
n = int(sp[0])
D = int(sp[1])
h = []
fh = []
num = []
mx = []
mn = []
cd = 1
b = 0
for i in range(n):
    h.append(int(input()))
num.append([h[0]])
mx.append(h[0])
mn.append(h[0])
for i in range(1,n):
    for j in range(cd):
        if mn[cd-j-1] < h[i] - D or mx[cd-j-1] > h[i] + D:
            if j == 0:
                num.append([h[i]])
                mx.append(h[i])
                mn.append(h[i])
                cd += 1
            else:
                num[cd-j].append(h[i])
                if mn[cd-j] > h[i]:
                    mn[cd-j] = h[i]
                elif mx[cd-j] < h[i]:
                    mx[cd-j] = h[i]
            h[i] = -1
            break
    if not h[i] == -1:
        num[0].append(h[i])
        if mn[0] > h[i]:
            mn[0] = h[i]
        elif mx[0] < h[i]:
            mx[0] = h[i]
for i in range(cd):
    list.sort(num[i])
    for j in range(len(num[i])):
        print(num[i][j])
```

最大最小整数

```python
import math

def maxx(p,q):#返回p，q中较大者
    lenth=min(len(p),len(q))
    for i in range(lenth):
        if p[i]>q[i]:
            return p
        if q[i]>p[i]:
            return q
    pp=p+q
    qq=q+p
    if pp>=qq:
        return p
    else:
        return q


def slicer(r):#[r,l)，返回已排序好的序列
    lenth=len(r)
    if lenth==1:
        return r
    else:
        mid=math.ceil(lenth/2)
        right=slicer(r[0:mid])
        left=slicer(r[mid:lenth])
        s=[]
        while len(right)!=0 and len(left)!=0:
            x=maxx(right[0],left[0])
            s.append(x)
            if x==right[0]:
                del right[0]
            else:
                del left[0]
        s.extend(right)
        s.extend(left)
        return s

n=int(input())
a=[str(i) for i in input().split()]
s=slicer(a)
b=s[0]
c=s[n-1]
for i in range(1,n):
    b+=s[i]
    c+=s[n-i-1]
print(b,c)
```

T-prime

```python
import math

prime={}
for i in range(1000001):
    prime[i]=1
for i in range(2,1000001):
    if prime[i]:
        for j in range(i*i,1000001,i):
            prime[j]=0
prime[1]=0

n=int(input())
a=[int(i) for i in input().split()]
for i in a:
    aa=math.ceil(math.sqrt(i))
    if aa*aa==i and prime[aa]:
        print("YES")
    else:
        print("NO")
```

### 数字三角形

```python
from functools import lru_cache
@lru_cache(maxsize = 128)
def lyj(i,j):
    if i==n-1:
        return a[i][j]
    else:
        return a[i][j]+max(lyj(i+1,j),lyj(i+1,j+1))

n=int(input())
a=[]
for i in range(n):
    a.append([int(i) for i in input().split()])
print(lyj(0,0))
```

### 世界杯只因

```python
数院胡睿诚
# 就是从左往右扫，一轮一轮的扫

# 比如现在这一轮结束之后第一个没被盖住的是x,你就继续扫能盖住x的，
# 在所有能盖住x的里面挑右端点最靠右边的，把它选进来，然后更新第一个没被盖住的点，进入下一轮
#
# 其实这个算法对于任给一族区间要找最小覆盖的问题都对

N = int(input())
a = list(map(int, input().split()))
intervals = [(max(0, i-a[i]), min(N-1, i+a[i])) for i in range(N)]
intervals.sort()

ans = 0
right = 0
temp = -1
index = 0
while index < N and right < N:
    while index < N and intervals[index][0] <= right:
        temp = max(temp, intervals[index][1])
        index += 1
    right = temp + 1
    ans += 1

print(ans)

```

### 八皇后

```python
import copy

def queen(hang,a):
    global ans
    for i in range(1,9):
        a[hang]=i
        if hang==7:
            if check(hang,a):
                ans.append(copy.deepcopy(a))
        else:
            if check(hang,a):
                queen(hang+1,a)       

def check(hang,a):
    for i in range(hang):
        if a[i]==a[hang] or a[i]-a[hang]==i-hang or a[i]-a[hang]==hang-i:
            return 0
    return 1
   

ans=[]
queen(0,[0,0,0,0,0,0,0,0])

t=int(input())
for _ in range(t):
    n=int(input())
    print(''.join(str(i) for i in ans[n-1]))

```

二分查找

<img src="C:\Users\40864\AppData\Roaming\Typora\typora-user-images\image-20231227142217618.png" alt="image-20231227142217618" style="zoom: 50%;" />

当前队列中位数

```python
import bisect
n=int(input())
l=[]
ll=[]
m=0
mm=0
for i in range(n):
    a=input()
    if a[0]=='a':
        b=int(a[4:])
        bisect.insort_left(l,int(b))
        ll.append(b)
    if a=='query':
        if (len(l)-m)%2==1:
            print(l[m+(len(l)-m)//2])
        else:
            ans=l[m+(len(l)-m)//2-1]+l[m+(len(l)-m)//2]
            if ans%2==0:
                print(ans//2)
            else:
                print(ans/2)
    if a=='del':
        d=ll[mm]
        mm+=1
        del l[bisect.bisect_left(l,d)]
```

### 田忌赛马

```python
n=int(input())
while n!=0:
    tian=[int(i) for i in input().split()]
    king=[int(i) for i in input().split()]
    tian.sort()
    king.sort()
    i=0
    j=0
    k=n-1
    l=n-1
    ans=0
    while i<=l:
        #print(i,j,k,l)
        if tian[i]>king[j]:
            i+=1
            j+=1
            ans+=1
        else:
            if tian[l]>king[k]:
                l-=1
                k-=1
                ans+=1
            else:
                if tian[i]==king[k]:
                    i+=1
                    k-=1
                else:
                    k-=1
                    i+=1
                    ans-=1
            
    print(ans*200)
    n=int(input())
```

### 剪绳子

```python
import bisect
n=int(input())
l=[int(i) for i in input().split()]
l.sort()
ans=0
while len(l)>1:
    t=l.pop(0)+l.pop(0)
    bisect.insort(l,t)
    ans+=t
print(ans)
```

| 二进制   | 十进制 | 十六进制 | 字符/缩写                                    | 解释                               |
| -------- | ------ | -------- | -------------------------------------------- | ---------------------------------- |
| 00000000 | 0      | 00       | NUL (NULL)                                   | 空字符                             |
| 00000001 | 1      | 01       | SOH (Start Of Headling)                      | 标题开始                           |
| 00000010 | 2      | 02       | STX (Start Of Text)                          | 正文开始                           |
| 00000011 | 3      | 03       | ETX (End Of Text)                            | 正文结束                           |
| 00000100 | 4      | 04       | EOT (End Of Transmission)                    | 传输结束                           |
| 00000101 | 5      | 05       | ENQ (Enquiry)                                | 请求                               |
| 00000110 | 6      | 06       | ACK (Acknowledge)                            | 回应/响应/收到通知                 |
| 00000111 | 7      | 07       | BEL (Bell)                                   | 响铃                               |
| 00001000 | 8      | 08       | BS (Backspace)                               | 退格                               |
| 00001001 | 9      | 09       | HT (Horizontal Tab)                          | 水平制表符                         |
| 00001010 | 10     | 0A       | LF/NL(Line Feed/New Line)                    | 换行键                             |
| 00001011 | 11     | 0B       | VT (Vertical Tab)                            | 垂直制表符                         |
| 00001100 | 12     | 0C       | FF/NP (Form Feed/New Page)                   | 换页键                             |
| 00001101 | 13     | 0D       | CR (Carriage Return)                         | 回车键                             |
| 00001110 | 14     | 0E       | SO (Shift Out)                               | 不用切换                           |
| 00001111 | 15     | 0F       | SI (Shift In)                                | 启用切换                           |
| 00010000 | 16     | 10       | DLE (Data Link Escape)                       | 数据链路转义                       |
| 00010001 | 17     | 11       | DC1/XON (Device Control 1/Transmission On)   | 设备控制1/传输开始                 |
| 00010010 | 18     | 12       | DC2 (Device Control 2)                       | 设备控制2                          |
| 00010011 | 19     | 13       | DC3/XOFF (Device Control 3/Transmission Off) | 设备控制3/传输中断                 |
| 00010100 | 20     | 14       | DC4 (Device Control 4)                       | 设备控制4                          |
| 00010101 | 21     | 15       | NAK (Negative Acknowledge)                   | 无响应/非正常响应/拒绝接收         |
| 00010110 | 22     | 16       | SYN (Synchronous Idle)                       | 同步空闲                           |
| 00010111 | 23     | 17       | ETB (End of Transmission Block)              | 传输块结束/块传输终止              |
| 00011000 | 24     | 18       | CAN (Cancel)                                 | 取消                               |
| 00011001 | 25     | 19       | EM (End of Medium)                           | 已到介质末端/介质存储已满/介质中断 |
| 00011010 | 26     | 1A       | SUB (Substitute)                             | 替补/替换                          |
| 00011011 | 27     | 1B       | ESC (Escape)                                 | 逃离/取消                          |
| 00011100 | 28     | 1C       | FS (File Separator)                          | 文件分割符                         |
| 00011101 | 29     | 1D       | GS (Group Separator)                         | 组分隔符/分组符                    |
| 00011110 | 30     | 1E       | RS (Record Separator)                        | 记录分离符                         |
| 00011111 | 31     | 1F       | US (Unit Separator)                          | 单元分隔符                         |
| 00100000 | 32     | 20       | (Space)                                      | 空格                               |
| 00100001 | 33     | 21       | !                                            |                                    |
| 00100010 | 34     | 22       | "                                            |                                    |
| 00100011 | 35     | 23       | #                                            |                                    |
| 00100100 | 36     | 24       | $                                            |                                    |
| 00100101 | 37     | 25       | %                                            |                                    |
| 00100110 | 38     | 26       | &                                            |                                    |
| 00100111 | 39     | 27       | '                                            |                                    |
| 00101000 | 40     | 28       | (                                            |                                    |
| 00101001 | 41     | 29       | )                                            |                                    |
| 00101010 | 42     | 2A       | *                                            |                                    |
| 00101011 | 43     | 2B       | +                                            |                                    |
| 00101100 | 44     | 2C       | ,                                            |                                    |
| 00101101 | 45     | 2D       | -                                            |                                    |
| 00101110 | 46     | 2E       | .                                            |                                    |
| 00101111 | 47     | 2F       | /                                            |                                    |
| 00110000 | 48     | 30       | 0                                            |                                    |
| 00110001 | 49     | 31       | 1                                            |                                    |
| 00110010 | 50     | 32       | 2                                            |                                    |
| 00110011 | 51     | 33       | 3                                            |                                    |
| 00110100 | 52     | 34       | 4                                            |                                    |
| 00110101 | 53     | 35       | 5                                            |                                    |
| 00110110 | 54     | 36       | 6                                            |                                    |
| 00110111 | 55     | 37       | 7                                            |                                    |
| 00111000 | 56     | 38       | 8                                            |                                    |
| 00111001 | 57     | 39       | 9                                            |                                    |
| 00111010 | 58     | 3A       | :                                            |                                    |
| 00111011 | 59     | 3B       | ;                                            |                                    |
| 00111100 | 60     | 3C       | <                                            |                                    |
| 00111101 | 61     | 3D       | =                                            |                                    |
| 00111110 | 62     | 3E       | >                                            |                                    |
| 00111111 | 63     | 3F       | ?                                            |                                    |
| 01000000 | 64     | 40       | @                                            |                                    |
| 01000001 | 65     | 41       | A                                            |                                    |
| 01000010 | 66     | 42       | B                                            |                                    |
| 01000011 | 67     | 43       | C                                            |                                    |
| 01000100 | 68     | 44       | D                                            |                                    |
| 01000101 | 69     | 45       | E                                            |                                    |
| 01000110 | 70     | 46       | F                                            |                                    |
| 01000111 | 71     | 47       | G                                            |                                    |
| 01001000 | 72     | 48       | H                                            |                                    |
| 01001001 | 73     | 49       | I                                            |                                    |
| 01001010 | 74     | 4A       | J                                            |                                    |
| 01001011 | 75     | 4B       | K                                            |                                    |
| 01001100 | 76     | 4C       | L                                            |                                    |
| 01001101 | 77     | 4D       | M                                            |                                    |
| 01001110 | 78     | 4E       | N                                            |                                    |
| 01001111 | 79     | 4F       | O                                            |                                    |
| 01010000 | 80     | 50       | P                                            |                                    |
| 01010001 | 81     | 51       | Q                                            |                                    |
| 01010010 | 82     | 52       | R                                            |                                    |
| 01010011 | 83     | 53       | S                                            |                                    |
| 01010100 | 84     | 54       | T                                            |                                    |
| 01010101 | 85     | 55       | U                                            |                                    |
| 01010110 | 86     | 56       | V                                            |                                    |
| 01010111 | 87     | 57       | W                                            |                                    |
| 01011000 | 88     | 58       | X                                            |                                    |
| 01011001 | 89     | 59       | Y                                            |                                    |
| 01011010 | 90     | 5A       | Z                                            |                                    |
| 01011011 | 91     | 5B       | [                                            |                                    |
| 01011100 | 92     | 5C       | \                                            |                                    |
| 01011101 | 93     | 5D       | ]                                            |                                    |
| 01011110 | 94     | 5E       | ^                                            |                                    |
| 01011111 | 95     | 5F       | _                                            |                                    |
| 01100000 | 96     | 60       | `                                            |                                    |
| 01100001 | 97     | 61       | a                                            |                                    |
| 01100010 | 98     | 62       | b                                            |                                    |
| 01100011 | 99     | 63       | c                                            |                                    |
| 01100100 | 100    | 64       | d                                            |                                    |
| 01100101 | 101    | 65       | e                                            |                                    |
| 01100110 | 102    | 66       | f                                            |                                    |
| 01100111 | 103    | 67       | g                                            |                                    |
| 01101000 | 104    | 68       | h                                            |                                    |
| 01101001 | 105    | 69       | i                                            |                                    |
| 01101010 | 106    | 6A       | j                                            |                                    |
| 01101011 | 107    | 6B       | k                                            |                                    |
| 01101100 | 108    | 6C       | l                                            |                                    |
| 01101101 | 109    | 6D       | m                                            |                                    |
| 01101110 | 110    | 6E       | n                                            |                                    |
| 01101111 | 111    | 6F       | o                                            |                                    |
| 01110000 | 112    | 70       | p                                            |                                    |
| 01110001 | 113    | 71       | q                                            |                                    |
| 01110010 | 114    | 72       | r                                            |                                    |
| 01110011 | 115    | 73       | s                                            |                                    |
| 01110100 | 116    | 74       | t                                            |                                    |
| 01110101 | 117    | 75       | u                                            |                                    |
| 01110110 | 118    | 76       | v                                            |                                    |
| 01110111 | 119    | 77       | w                                            |                                    |
| 01111000 | 120    | 78       | x                                            |                                    |
| 01111001 | 121    | 79       | y                                            |                                    |
| 01111010 | 122    | 7A       | z                                            |                                    |
| 01111011 | 123    | 7B       | {                                            |                                    |
| 01111100 | 124    | 7C       | \|                                           |                                    |
| 01111101 | 125    | 7D       | }                                            |                                    |
| 01111110 | 126    | 7E       | ~                                            |                                    |
| 01111111 | 127    | 7F       | DEL (Delete)                                 | 删除                               |

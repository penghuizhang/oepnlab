# oepnlab

INDIRECT(CONCATENATE($A5,"!",I$3))

这是一个动态引用的公式。CONCATENATE($A5,"!",I$3)将字符串连起来，相当于$A5&"!"&I$3。
然后INDIRECT建立文本形式的引用。
举例说：$A5中的字符为"sheet2"，I$3中的字符是D2，那么公式的运算过程为：
=INDIRECT(CONCATENATE($A5,"!",I$3))
=INDIRECT($A5&"!"&I$3)
=INDIRECT("sheet2!D2")
=D2
公式得到D2的值，

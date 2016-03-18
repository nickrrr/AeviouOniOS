# AeviouOniOS
aeviou输入法的iOS版本的前台部分

最后更新时间： 2016-03-18

使用说明：
1.由于用的是xocde 6.3（for iOS8），当前版本苹果对自定义键盘的支持还不是很好，不能获取默认键盘的frame和bounds，可能需要调节一下键盘的宽高尺寸，在KeyboardViewController中设置即可。在for iOS9及以后的版本中就没有这个问题

完成功能可供验证：
1.hexkeyBoard：
1）单击字母键，单击特殊符号键（逗号，句号等）
2）滑动，退回滑动
3）滑动按键判定
4）当z，c，s 滑动至zh，ch，sh 将slidepath路径起始拷贝至 zh ch sh 例子：chong
5）补充需要的ng 并设为next 例子：gang与chong的区别
6）aoe键的滑动以 a，o或e作为路径起点
6）切换至其他输入法（按“英”）
7）切换至输入法中内置的symbolkeyBoard

2.symbolkeyBoard
1）单击普通符号，特殊符号
2）page键 （“1/2” "2/2")进行symbolkeyBoard内部页面切换及重绘
3）return键 （“返回”）切换到hexkeyBoard
4）对于key（name：“29”，id：“30”）即第一页中的“-_-”键特殊处理和绘制

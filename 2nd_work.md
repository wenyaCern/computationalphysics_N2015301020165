# 在屏幕上用字符画打印自己的名字，并让它“动起来”

## 最终成果
![image](https://github.com/amanaaaa/computationalphysics_N2015301020165/blob/master/2en_work.gif)

## 使用语句包括

   - print('\n')
   - import time 
         time.sleep()
   - import os
         os.system('cls')
         
## 实验的过程
   - 首先是参照了C语言中‘奔跑的字母’这个小程序，考虑到需要用循环语句、时间变量和空格及清除字符串的语句
   
   - 但在尝试把C语言对应成python后，由于自己的编程功底实在太弱，大概就是菜鸟小白级别，于是只是用了最简单的print加时间停顿加清除界面；
     在清除这部分还遇到了一些麻烦，最开始只写了两句print中间加一个清除，清除语句之后的程序运行完就结束，因此误认成清除之后程序无法再进行下一步操作，
     一度放弃该方法。
     
   - 在学习python时，了解到另外一种'\r'即将末尾的光标移动到该行最前的方法，运用了如下语句：
      
      'print('information', end='\r')'
      
      'import time'
      
      'time.sleep(1)'
      
      'print(end='\raaaaaaaaaaa')'
      
        该语句可以在1s后将“information”刷新为“aaaaaaaaaaa”,但一旦加上换行符，就只能替换上一个print的最后一行；后来了解到python的设计是仿照老式打印         机，按行处理打印内容的， '\r' 指令只能将光标移动到本行之前，不能处理上一行及以前的字符串，放弃。
     
   - 最开始是看到b站大神把视频转换称动态字符画，代码很复杂。

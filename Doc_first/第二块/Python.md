# Python进阶

[TOC]

## 多任务

### 线程

#### 创建一个线程并运行

```python
import threading
import time


def print1():
    for i in range(3):
        print("------1----")
        
        # 推迟调用线程的运行，进程挂起的时间, 秒
        time.sleep(1)

def print2():
    for i in range(3):
        print("------2----")
        time.sleep(1)


def main():

    # 创建一个线程对象，设置线程的入口函数，
    # 参数：入口函数名字，这个函数执行完，标志着这个子线程结束
    t1 = threading.Thread(target = print1)
    t2 = threading.Thread(target = print2)
    
    # 启动线程，start()函数表示启动/开始调度这个线程，执行子线程入口函数
    t1.start()
    t2.start()
    
    
    while True:
        
        # 在这个循环体中，print1，print2一直在执行，直接执行结束，死循环
        # enumerate()返回一个列表，里面有所有线程
        # 这个程序应该有3个线程，主线程，2个子线程
        # 但是显示有9个线程，可能和这个集成环境有关
        info = threading.enumerate()
        l = len(info)
       # print(l)
         

if __name__ == "__main__":
    main()
```

#### 创建一个线程对象

```python

import threading
import time

# 定义一个线程对象，实现自己的任务代码
class MyThread(threading.Thread):
    def run(self):
        for i in range(3):
            
            print("----run %d----" % i)
            time.sleep(1)

            
def main():
    
    # 实例化类对象
    t1 = MyThread()
    
    # 类对象调用start()方法，开始一个关于这个类的子线程
    # start()自动调用类中的run()方法，run在调用类中的其他方法，完成相关任务
    # 启动这个线程对象，run()会不停的被调用
    t1.start()
    

if __name__ == "__main__":
    main()

```







## PyQt

在anaconda中安装PyQt的库，可以用Qt的designer来设计界面，然后使用pyuic5.exe(.bat)来把ui文件转成对应的py文件（安装完PyQt库后，就有pyuic），转换步骤如下

> 1.打开cmd窗口（shift+右键）
>
> 2.输入：pyuic5.bat xx.ui -o xx.py

需要注意的是，如果提示找不到pyuic5命令，那么可以添加环境变量，或者可以把这个ui文件复制到pyuic5所在目录，然后在这个目录中，执行上述步骤。使用listary查找pyuic5所在路径，目前我的机器是：

> F:\ProgramData\Anaconda3\Library\bin\pyuic5.bat
>
> F:\ProgramData\Anaconda3\pkgs\pyqt-5.9.2-py37h6538335_2\Library\bin\pyuic5.bat

我用的是上面第一个目录

或者使用pycharm的外部工具，但是需要配置，出错的话不好查。前后配置果两次，第一次成功，第二次失败，不想搞得那么复杂，不打算用pytcharm了，还是anaconda香啊。






















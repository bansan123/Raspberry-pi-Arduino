#Raspberry Pi + Arduino USB对接方式
关于树莓派与Arduino Uno如何对接，网络上的资料很少，经本人研究三天终于成功了，总结个教程。它们实现对接的方式至少有三种(USB方式对接、GPIO方式对接、 I2C方式对接、其他)。本文根据自己的经验记述一下USB对接过程。

* 1 插上两个Arduion Uno与树莓派 的USB 然后 在树莓派输入:

  `ls /dev/tty*`

  查看有没有ttyACM0 这个文件(注只有在两个硬件USB互连的情况下才会有这个。如果两者没有连接是不会有的) 最新的系统一般都会自动生成。看到ttyACMO就说明二者可以通讯了 接下来上测试代码
  Arduino代码见testaduino
  Raspberry Pi代码见testraspberry

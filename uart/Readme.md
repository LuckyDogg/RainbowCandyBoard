把扩展板的 USB TO UART 连接到电脑，设置电脑的串口软件（可使用 PuTTY 等软件监 视串口） ，选择正确的串口号，波特率设置为 115200。 电脑通过串口向树莓派发送数据，树莓 派在接收到这些数据之后，会把数据通过串口传送回电脑。因此，从电脑端向树莓派发送的数据 会回显在电脑端的串口监视软件中。
请根据自己的板子选择不同的版本。

### 释放串口  
执行如下命令进入树莓派配置   
`sudo raspi-config`
选择 Interfacing Options  ->Serial ->no -> yes 关闭串口调试功能,打开串口  

注：如果是树莓派3B，板载的串口ttyAMA0作为蓝牙使用，用户串口端口改为ttySO。如下程序也类似，如果是到的树莓派3B,ttyAMA0需改为ttyS0。

[RainbowCandyBoard.pdf](https://github.com/MrzhangF1ghter/RainbowCandyBoard/blob/master/schematic/RainbowCandyBoard_Rev2.0.pdf)<br>
<img src="https://img.alicdn.com/imgextra/i4/1887229091/O1CN012H1j62SbmCMZ7bT_!!1887229091.png" width=50% height=50%/><br>
<img src="https://img.alicdn.com/imgextra/i3/1887229091/O1CN012H1j61aNzLFVnFZ_!!1887229091.png" width=50% height=50%/><br>


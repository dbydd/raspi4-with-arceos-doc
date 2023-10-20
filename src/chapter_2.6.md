# 实验二：通过 UART0 驱动小车

1. 在ArceOS目录下，输入：

   ```shell
   make A=apps/boards/raspi4 ARCH=aarch64 PLATFORM=aarch64-raspi4 LOG=debug SMP=4
   ```

   编译出ArceOS在raspi4 上的一个镜像raspi4_aarch64-raspi4.bin。

2. 在rust-raspberrypi-OS-tutorials/06_uart_chainloader中输入：

   ```shell
   BSP=rpi4 make
   ```

   编译生成一个kernel8.img文件。

3. 把 kernel8.img 和 raspi4_aarch64-raspi4.bin 通过 cat 命令拼接到一个 bin 文件中，仍然取名为 kernel8.img：

   ```
   cat ../rust-raspberrypi-OS-tutorials/06_uart_chainloader/kernel8.img apps/boards/raspi4/raspi4_aarch64-raspi4.bin > kernel8.img
   ```

4. 把新生成的 kernel8.img 拷贝到 sd 卡上，并且将树莓派串口连线与小车相连。
   
5. 打开树莓派电源，可以看到小车会走出一个方形的轨迹。
   
6. 修改代码，改变小车的运动轨迹。

   
至此，实验二结束，最终提交小车运行的视频及相关代码。




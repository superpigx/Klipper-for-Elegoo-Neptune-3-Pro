# 前言
我很早之前买了一台海王星3pro的打印机，但是我买了以后就开始都变成了高速打印机，可惜的我过了退货期限
# 改装
我就开始了我的打印机改装之路，我先刷了klipper固件，然后开始了我的调整配置阶段

# 刷机
 对于 ZNP Robin Nano DW v2.2 主板：
 - 使用处理器型号 STM32F401 进行编译。
 - 选择 32KiB 引导加载程序，
 - 选择（串口（on # USART1 PA10/PA9）作为通信接口。
 - 如果要使用 J17 上的串口 UART 引脚（wifi 部分），请选择（串口（on # USART2 PA3/PA2）
 请注意，“make flash”命令不适用于 ZNP Robin Nano DW v2.2 主板。运行“make”后，运行以下命令：
 cp out/klipper.bin out/ZNP_ROBIN_NANO.bin

 将文件输出/ZNP_ROBIN_NANO.bin复制到 SD 卡，然后使用该 SD 卡重新启动打印机。
# 后续
先这样吧定期更新吧，不是很会玩github 先这样吧！

# 时间表

2024年8月29日 创建仓库上传配置
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
 # 固件下载
 固件增添到了【klipper固件】里面可以下载了
# 后续
先这样吧，有空我再更新吧，不是很会玩github。老更新不上去！
后续再写一下各种调整的模板吧，慢慢研究玩吧
正好也给自己留个备份
# 说明
## 固件是直接从TheFeralEngineer库里弄来的，当然你也可自己编译一个新版本的，反正我用着没事
https://github.com/TheFeralEngineer/Klipper-for-Elegoo-Neptune-series-3D-Printers

## 配置文件也是不停修改也写了不少中文的注释，也有从别人那学习来的各种资料，忘了最早是谁修改的版本来着
## 里面使用了Klipper-Adaptive-Meshing-Purging，直接套用配置可能会出错，先装一下这个
https://github.com/kyleisah/Klipper-Adaptive-Meshing-Purging
# 时间表

2024年8月29日 创建仓库上传配置
2024年8月30日 更新固件，更新文档
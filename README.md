# co2lemp
A smart light that changes its emission color according to environmental conditions
項目            |  内容　|　IF
:-------------------------:|:-------------------------:|:-------------------------:
 MPU | STM32 Nucleo Board STM32F303K8 | -
CO2センサ| MH-Z19C | UART
温湿度センサ| AE-SHT31 | I2C
LED| OSTA71A1D-A | Digital-OUT / PWM
FLASH| W25Q16JVUXIQ | SPI
アナログボリューム | - | Analog-IN
DIP switch (4bit) | - | Digital-IN

 ### 最終成果物

<center><img src="https://github.com/ChouYuduki/co2lemp/blob/main/1.png" width="600"></center>


## 指標切り替え  
- **スイッチ切り替え** により LED の検出指標を変更
<center><img src="https://github.com/ChouYuduki/co2lemp/blob/main/2.png" width="400"></center>

- **室内の CO₂ 濃度・温度・湿度** を測定可能  




##  LED 色変化ルール（CO₂ 濃度）  
- **1000 未満**  →   🔵 青  
- **1000～1500** →   🟢 緑  
- **1500～2500** →   🟡 黄  
- **2500～3500** →   🔴 赤  
- **3500 以上**  →   🟣 紫  

##  リアルタイム表示  
- 各パラメータを **リアルタイムでディスプレイに表示**  
- 現在の検出指標も **確認可能**




### ESP32-C6 ULP mini PCB

This PCB design is based on [C6 design guidelines](https://docs.espressif.com/projects/esp-hardware-design-guidelines/en/latest/esp32c6/schematic-checklist.html) and uses the Buck converter schematic of Seeed XIAO C6 [SGM6029](https://www.sg-micro.com/product/SGM6029)

> The SGM6029 family is a low voltage, efficient and miniature synchronous Buck converter with ultra-low quiescent current. Operating at high switching frequency (4.0MHz, TYP), miniature inductors and capacitors can be used to achieve minimal solution size.


#### Using low GPIOs to be able to access them from ULP

```
IO Description
0 EPD_MOSI
1 EPD_CLK
2 EPD_CS
3 EPD_DC
4 EPD_BSY
5 EPD_RST
6 SCL --> I2C ↘
7 SDA --> I2C connected to RV2032 RTC
```

![CPU schematic](/components/imgs/1.0_CPU_sch.png)

### Push buttons GPIOs (optional side switches)

```
IO Description
19 Left  SW1 
20 Right SW2
18 Right SW3
```

![SW placement](/components/imgs/1.0-back.png)

### 3D-Preview

![Front PCB preview](/components/imgs/1.0-front.png)

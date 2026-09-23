## cap-moist-sens
# Adafruit I2C Capacitive Moisture Sensor

Testing the moisture sensors when hooked up to a Raspberry Pi 3 via a 5 post passive  hub.

# Detect the Sensors
```
don@raspberrypi-3-lab:~ $ sudo i2cdetect -y 1
     0  1  2  3  4  5  6  7  8  9  a  b  c  d  e  f
00:                         -- -- -- -- -- -- -- --
10: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
20: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
30: -- -- -- -- -- -- 36 37 38 39 -- -- -- -- -- --
40: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
50: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
60: -- -- -- -- -- -- -- -- -- -- -- -- -- -- -- --
70: -- -- -- -- -- -- -- --
```

# Sample Data

I collected data on four different sensors with addresses 0x36, 0x37, 0x38, 0x39.

Here's the average values when in air and then immersed in tap water.

| Sensor | Average Air | Average Water|
|:------:|:-----------:|:------------:|
| 0x36   | 340         | 469          |
| 0x37   | 378         | 460          |
| 0x38   | 343         | 457          |
| 0x39   | 350         | 485          |



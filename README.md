## How to download wiringROCK960

```
# apt-get update
# apt-get install -y git
# git clone https://github.com/Anuo-shuo/wiringROCK960.git
```

## How to build wiringROCK960

```
# cd wiringROCK960
# ./build clean
# ./build 
```

## How to use wiringROCK960

```
# gpio readall
# gpio mode 15 out
# gpio write 15 1
# gpio readall
```

---
## The output of the gpio readall command 
### ROCK960

 ```
 +------+-----+-------------+------+---+  ROCK960 +---+---+--+--------------+-----+------+
 | GPIO | wPi |     Name    | Mode | V | Physical | V | Mode |     Name     | wPi | GPIO |
 +------+-----+-------------+------+---+----++----+---+------+--------------+-----+------+
 |      |     |         GND |      |   |  1 || 2  |   |      | GND          |     |      |
 |  112 |   0 |   UART3_CTS |   IN | 1 |  3 || 4  |   |      | PMIC_PWRON   |     |      |
 |  111 |   1 |    UART3_TX |  OUT | 0 |  5 || 6  |   |      | RESET_L      |     |      |
 |  110 |   2 |    UART3_RX |   IN | 1 |  7 || 8  | 0 | OUT  | SPI0_CLK     | 3   | 102  |
 |  113 |   4 |   UART3_RTS |   IN | 1 |  9 || 10 | 0 | ALT3 | SPI0_RX      | 5   | 97   |
 |   40 |   6 |    UART4_TX |  OUT | 0 | 11 || 12 | 1 | ALT3 | SPI0_CS      | 7   | 103  |
 |   39 |   8 |    UART4_RX |  OUT | 0 | 13 || 14 | 0 | OUT  | SPI0_TX      | 9   | 101  |
 |   74 |  10 |    I2C6_SCL |  OUT | 0 | 15 || 16 | 0 | IN   | I2S0_LRCK_TX | 11  | 122  |
 |   73 |  12 |    I2C6_SDA |  OUT | 0 | 17 || 18 | 0 | OUT  | I2S0_SCLK    | 13  | 120  |
 |  130 |  14 |    I2C1_SCL |  OUT | 0 | 19 || 20 | 0 | OUT  | I2S0_SDO0    | 15  | 127  |
 |  129 |  16 |    I2C1_SDA |  OUT | 0 | 21 || 22 | 0 | IN   | I2S0_SDI0    | 17  | 123  |
 |    6 |  18 | GPIO0_A6_IR |  OUT | 0 | 23 || 24 | 0 | OUT  | GPIO0_A2     | 19  | 2    |
 |   41 |  20 |    GPIO1_B1 |  OUT | 1 | 25 || 26 | 1 | OUT  | GPIO1_B2     | 21  | 42   |
 |  121 |  22 |    GPIO3_D1 |   IN | 0 | 27 || 28 | 1 | OUT  | GPIO4_A0     | 23  | 128  |
 |  124 |  24 |    GPIO3_D4 |   IN | 0 | 29 || 30 | 1 | OUT  | GPIO4_A3     | 25  | 131  |
 |  125 |  26 |    GPIO3_D5 |   IN | 0 | 31 || 32 | 1 | OUT  | GPIO4_A4     | 27  | 132  |
 |   50 |  28 |    GPIO1_C2 |   IN | 1 | 33 || 34 | 1 | OUT  | GPIO1_C7     | 29  | 55   |
 |      |     |        1.8V |      |   | 35 || 36 |   |      | 12V          |     |      |
 |      |     |          5V |      |   | 37 || 38 |   |      | 12V          |     |      |
 |      |     |         GND |      |   | 39 || 40 |   |      | GND          |     |      |
 +------+-----+-------------+------+---+----++----+---+------+--------------+-----+------+
 | GPIO | wPi |     Name    | Mode | V | Physical | V | Mode |     Name     | wPi | GPIO |
 +------+-----+-------------+------+---+  ROCK960 +---+---+--+--------------+-----+------+
```

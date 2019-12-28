# robosys2019 - 課題1
17C1702　大塚文貴

## 概要
LEDが点灯、消灯を3回繰り返すプログラムで、入力する数字(1~9)によってLEDの点灯時間が変わります

## 使用するもの
Raspberry Pi 3 Model B+  
LED   
抵抗　100Ω  

## 使い方
環境構築
```
git clone https://github.com/otsuka-fumiki/robosys2019.git
cd robosys2019
make
sudo insmod myled.ko
sudo chmod 666 /dev/myled0
```
点灯させたい時間を入力(例：動画の場合)
1秒点灯して消灯を3回繰り返す
```
echo 1 > /dev/myled0
```
5秒点灯して消灯を3回繰り返す
```
echo 5 > /dev/myled0
```

## 動画
https://youtu.be/gjKGY2bcYSA

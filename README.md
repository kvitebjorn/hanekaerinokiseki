# hanekaerinokiseki 跳ね返りの軌跡
Breakout clone for GameBoy


To build, run the following command, assuming you set up `rgbasm`:

```
rgbasm -L -o main.o main.asm &&
rgblink -o hanekaerinokiseki.gb main.o &&
rgbfix -v -p 0xFF hanekaerinokiseki.gb
```


Add this line for sym links when debugging:

```
&& rgblink -n hanekaerinokiseki.sym main.o
```
# Yulong d200 headphones amplifier repair guide
We've got Yulong D200 with broken headphones amplifier.

![yulong d200](d200/IMG_5738.JPG)
![yulong d200 back side](d200/IMG_5737.JPG)

It have [class B](https://en.wikipedia.org/wiki/Push%E2%80%93pull_output) power amplifier stage on matched pair of [MJD243](doc/MJD243-D.PDF) with negative feedback from output to [OP275](doc/OP275.pdf) inverting input.

![yulong d200 headphones amplifier topology](d200/IMG_5732.JPG)

Spending some time on reverse-engineering the output stage schematics we came to the following picture. It might be not quite exact and a bit dirty, but it gives a picture of the actual output stage schematics.

![yulong d200 output stage schematics](d200/IMG_5731.jpg)

I was unable to determine the exact type of transistors in preamp stage, but got its characteristics, by measuring it on working channel.

Q2=Q7=Q9=Q4 are bipolar NPN transistors, which have the following characteristics
![yulong d200 output stage schematics, NPN preamp characteristics](d200/IMG_5728.JPG)

Q3=Q6=Q8=Q5 are bipolar PNP transistors, which have the following characteristics
![yulong d200 output stage schematics, PNP preamp characteristics](d200/IMG_5730.JPG)

Finaly I ended up by replacing Q2 with [BC847B](doc/BC847_SER.pdf) and R84 with 27 Ohm resistor.

## Yulong images

![yulong d200 back side](d200/IMG_5727.JPG)
![yulong d200 back side](d200/IMG_5734.JPG)
![yulong d200 back side](d200/IMG_5735.JPG)
![yulong d200 back side](d200/IMG_5736.JPG)
![yulong d200 back side](d200/IMG_5739.JPG)

## More info about yulong products

http://www.qobuz.com/gb-en/info/hi-res-guide/yulong-sabre-da8ii-solid177720

https://hi-news.ru/audio/obzor-capa-i-usilitelya-dlya-naushnikov-yulong-d200.html

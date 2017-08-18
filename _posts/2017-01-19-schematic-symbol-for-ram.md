---
title: Schematic symbol for RAM
layout: post
category: SBC
---

I started the day with full enthusiasm only to realise there is no library for the RAM I chose. Fortunately, KiCad comes with BGA-96 package with the ball pitch and diameter I need. Also, the pins are named with their column and row numbers i.e. A1,A2,A3.....,B1,B2,B3,.... which is the standard notation for BGA package. Now, all I have to do is create a schematic symbol and map the pins with their respective column and row numbers by looking at the datasheet and KiCad will map the symbol with the footprint. Piece of cake, right? Well, I thought so too, but mapping 96 pins with their respective positions is not easy no matter how it sounds. It is not tough but it is menial.
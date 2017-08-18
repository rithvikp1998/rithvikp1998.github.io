---
title: Schematic.....Done
layout: post
category: SBC
---

Finally, the schematic part of the circuit is over. I chose not to use terminal resistors as they not only increase the complexity of the board, most people and evaluation module designs didn't use them and had satisfactory result. And when I calculated, the allowed length of the trace before lumped circuit assumption fails turned out to be 15cm at 200MHz. So, I tentatively chose not to go with them. Also, I had tough time figuring out I/O buffers, by-pass capacitors and ferrite beads. I learnt a lot already and the only remaining part of the schematic is the debugging pins that should be routed. With that and other minor corrections that I would do as I proceed down the road aside, the schematic looks beautiful (to me).
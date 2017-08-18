---
title: Damn! I made a mistake
layout: post
category: SBC
---

Earlier today, I posted about how the designing part is over and all that is left is some tweaks. One of the tweaks is matching trace lengths which is crucial to maintain a sync between clock and other signals. I routed all the signals thinking that I would match the lengths after I complete the rest of the design. Now, thanks to the vias and the 4-layer design, I'm not able to move the traces around. What I should have done is route and match the lengths before routing rest of the board or I should have chosen a 6-layer design or used some layout patterns that ensure matching trace lengths. I made a quick calculation of timing differences assuming a generous 20mm difference in trace lengths and it turned out to be 0.2 nano seconds(around 10% of 400Mhz clock time period). Now, I have two options, lower the clock and pray the board works which, theoretically, it should or redesign the board from the beginning which puts 5-day work down the drain. Let's see.
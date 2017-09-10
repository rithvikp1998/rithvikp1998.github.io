---
title: Ok, that didn't go well
layout: post
category: piTorrent
---

Well, it's been almost 72 hours and it's Sunday night. My challenge to complete this in 72 hours failed miserably and I am only half way through. The reasons include but not limited to:

I seriously overlooked the involvment of networking concepts in the project and I have NEVER worked on networking before so, voila. On one side, this is bad, because I spent several hours learning about sockets and messages and trying to figure out routing packets using my public IP etc. and time was the only important factor in the challenge. But there is a silver lining to everything and planned or unexpected, I learnt something about networking. May not be a lot. May not be thorough, but definitely a start.

The byte strings overwhelmed me. This is similar to above. The first time I opened a .torrent file was on Friday morning (By opened, I mean, tried to figure out what it contains). And it was daunting, especially since I was supposed to parse that file and the things I could read ended in the first few lines (which was all that was needed as one's not supposed to read and figure out the 20-byte SHA1 hashes associated with different pieces of the file which brings me to the third point).

I didn't use hashing before. I mean, I knew what it was, I knew before Friday that I might need to use it, but I didn't know how to use it. Especially, verifying if it was the correct hash ended up as a nightmare. To people who don't know about SHA1, a change in single character of the string can (and will) change the hash value completely(it is also one of the reasons why people use it, given the hashed value, it is impossible to figure out the original sentence without calculating the hash of every string that is valid given the use case). Calculating the SHA1 and sending it to the tracker as a parameter in the URL was straight-forward using Python's hashlib and requests library. However the real problem came when I tried to verify the value. There was no way I could verify the hash since I didn't have a separate reliable source which supplied the hash value and I ended up looking for an open source BitTorrent client written in Python, looked it's code, copied it(which BTW, is the only code I copied so far in this project) and calculated hashes from both codes and verified.

Despite all the setbacks, I really enjoyed the challenge and I don't want to leave this incomplete, so I decided to work on this for one more week, after which comes my mid semester exams followed by recess(I use a desktop in college, so nothing to work on when I'm at home) and after coming back from the recess, I'll go back to myOS and SBC because guess what, it's September already. Time really files.
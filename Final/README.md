# Final Project

<code>
d1 $ stack [<br>
  every (choose [4,5,6]) ((fast (choose [2,3])) . (degradeBy 0.2)) $<br>
  n "~ [28 27 26 28]"<br>
    # s "dr"<br>
    # squiz "<1.7 2 4 8 16>",<br>
  echo 4 0.125 0.8 $<br>
  s "[~ [bd:17 bd:17*[2 | 3 | [5 8]]]]"<br>
    # hpf sine # crush 8,<br>
  s "bd?"<br>
] # pan (fast 2 $ square) # lpf (range 1000 5000 $ sine)<br>
<br>
d2 $<br>
  every 4 (fast 2) $<br>
  s "<jungbass:8(5, 8) [jungbass:3 | jungbass:9]>"<br>
    # legato 0.8<br>
<br>
d3 $ stack [<br>
  sometimes (# speed 10) $<br>
  slow (choose [3,4]) $<br>
  degradeBy 0.2 $<br>
  n "12*[23 | 29 | 37]" # sound "cosmicg"<br>
    # gain 0.8,<br>
  s "cosmicg" # gain ((0.5 <~) $ slow 8 $ range 0.5 0.75 $ sine)<br>
]<br>
<br>
hush<br>
</code><br>

For this patch, I decided to make randomness a key driver for the production of music, by using degradeBy and by extensive use of random indexing. I started with a standard drum loop in d1, and added audio filter for extra ambience. I then used the jungbass sample with a euclidian pattern, and by random indexing. As a final layer, I added a stack of sound effects from the cosmicg samples, randomly changing their speed.
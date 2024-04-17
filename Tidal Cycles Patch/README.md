#Tidal Cycles Patch

<code>
d1 $ stack [s "[hh hh?]*8",<br>
slow 1.5 $ every 4 (fast 2) $ s "bd/2 bd ~" # gain 1.1,<br>
n (run 8) # s "amencutup"<br>
] # gain 0.85
<br><br>
let a p = fast 2 $ (0.25 <~) $ p
<br><br>
d2 $ every 4 a $ s "jungbass" # n (irand 19) # legato "[0.9 | 0.125]"
<br><br>
hush
</code>

<br>
I started with the broken hi-hat and the amen break in <code>d1</code>. To created rhythmic interest, I made a bass drum sequence over the "big 3," iterating over 1.5 cycles. I wanted to play random samples from the jungbass patch on top of that. When trying to pass multiple functions within <code>every</code>, in <code>d2</code>, I figured that I would have to create a custom pattern. To do this, I looked for custom functions in the Tidal Cycles documentation.
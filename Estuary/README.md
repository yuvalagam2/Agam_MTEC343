<h1>Estuary Group Project</h1>

<code>n (scale "major" "0 2 4 5") # s "moog" # pan sine</code>

<code>s "[hh hh hh ~] [] [] []"</code>

<code>stack [s "[hh hh hh ~] [hh hh hh ~] [hh hh hh ~] [cp hh hh cp?]",<br>
s "[bd] [bd ~ ~ bd] [~ bd] [sd]"] # gain 0.6
</code>

<code>n "0" # s "led" # pan sine</code>

<code>n "10" # s "ukulele" # gain 0.8</code>

<code>fast 8 $ n "7 2" # s "feelfx"</code>

<code>n "0" # s "padlong" # gain 0.2</code>

Our estuary group project is a collaborative live coding set that transitions through 4 sections based on auditory cues. It is a semi-composed performance, in that code is prewritten and sectional order is predetermined, but freedom is given to manipulate the parameters in real time as desired.

Sections<br>
1: Ambience and slow kick, cue "crow" into section 2<br>
2: Groove, denser rhythms, arps and scales, cue "seawolf" into section 3<br>
3: Weird noise from several samples and multiple meters, cue "panlong" into section 4<br>
4: Back to kick+fire
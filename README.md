# Pitch-Data

## Files

### CSV's
pitchData.csv: data for each pitch for our selected pitchers and all hitters

pitchDataUpdatedZone.csv: corresponds to pitchData.csv but for the updated zone

pitchData_rightHandedHitters.csv: data for each pitch for our selected pitchers and right handed hitters only (Original zone) 

### Swing JSONs
swingData.json: Json that holds the chance of a hit, out, strike, and foul indexed by what kind of pitch and which part of the 
zone the pitch ENDS UP in 

swingDataUpdatedZone.json: same as swingData.json but for updated zone

### Take JSONs
takeData.json: takeData\[intended location\]\[zone\] gives the probability that a pitch for the intended location ends up in zone

takeDataUpdatedZone.json: same as takeData.json but for updated zone

Original Zone: <br>
<pre>
+---+-----------+---+ 
|9  |     10    | 11|
|---+-----------+---|
|   | 0 | 1 | 2 |   |
|   |---+---+---|   |
|12 | 3 | 4 | 5 | 13|
|   |---+---+---|   |
|   | 6 | 7 | 8 |   |
|---+-----------+---|
|14 |     15    | 16|
+---+-----------+---+
</pre>

Updated Zone: <br>
<pre>
+---+-----------+---+
|9  |     10    | 11|
|   |-----------|   |
|   | 0 | 1 | 2 |   |
|   |---+---+---|   |
|---| 3 | 4 | 5 |---|
|   |---+---+---|   |
|   | 6 | 7 | 8 |   |
|   |-----------|   |
|12 |     13    | 14|
+---+-----------+---+
</pre>

# Pitch-Data

## Files

### CSV's
pitchData.csv: data for each pitch for our selected pitchers and all hitters

pitchDataUpdatedZone.csv: corresponds to pitchData.csv but for the updated zone

pitchData_rightHandedHitters.csv: data for each pitch for our selected pitchers and right handed hitters only (Original zone) 

pitchData_rightHandedHitters_withBatterID.csv: same as pitchData_rightHandedHitters.csv but with batter ID (for stratifying data later)

pitchData_rightHandedHitters_aboveAvgHitters.csv: same as pitchData_rightHandedHitters.csv but for only hitters with avg >= .250

pitchData_rightHandedHitters_belowAvgHitters.csv: same as pitchData_rightHandedHitters.csv but for only hitters with avg < .250

pitchData_AllPitchers.csv: analogous to pitchData.csv except with all pitchers

pitchData_AllPitchers_withBatterID.csv: analogous to pitchData_rightHandedHitters_withBatterID.csv

pitchData_allPitchers_aboveAvgHitters.csv: analogous to pitchData_rightHandedHitters_aboveAvgHitters.csv but with all pitchers

pitchData_allPitchers_belowAvgHitters.csv: analogous to pitchData_rightHandedHitters_belowAvgHitters.csv but with all pitchers


### Swing JSONs
swingData.json: Json that holds the chance of a hit, out, strike, and foul indexed by what kind of pitch and which part of the 
zone the pitch ENDS UP in 

swingData_rightHand.json: same as swingData.json but for right handed hitters only 

swingData_rightHand_aboveAvg.json: same as swingData.json but for right handed hitters only with batting avg >= .250

swingData_rightHand_belowAvg.json: same as swingData.json but for right handed hitters only with batting avg < .250

swingDataUpdatedZone.json: same as swingData.json but for updated zone

swingData_allPitchers_aboveAvg.json: analogous to swingData_rightHand_aboveAvg.json but with all pitchers

swingData_allPitchers_belowAvg.json: analogous to swingData_rightHand_belowAvg.json but with all pitchers


### Take JSONs
takeData.json: takeData\[intended location\]\[zone\] gives the probability that a pitch for the intended location ends up in zone

takeDataUpdatedZone.json: same as takeData.json but for updated zone

## Zones

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

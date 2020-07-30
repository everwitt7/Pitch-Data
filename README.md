# Pitch-Data

## Files

### CSVs
allPitchers_rightHitters_swingData_withBatterID.csv: old swing data for all pitchers and rhh

allPitchers_rightHitters_takeData_withBatterID.csv: old take data for all pitchers and rhh

all_pitchers_rhh_swing_data.csv.csv: current swing data for all pitchers and rhh

all_pitchers_rhh_take_data.csv.csv: current take data for all pitchers and rhh

raw_tensor_data_swing.csv: raw data needed to create tensors, had to split into swing and take to meet file size requirements

raw_tensor_data_take.csv: raw data needed to create tensors, had to split into swing and take to meet file size requirements

2019_raw_tensor_data_swing.csv: raw data needed to create tensors, had to split into swing and take to meet file size requirements. only 2019 data

2019_raw_tensor_data_take.csv: raw data needed to create tensors, had to split into swing and take to meet file size requirements. only 2019 data

batter_obp.csv: batter id to their empirical obp

pitcher_obp_against.csv: pitcher id to their opposing obp 

batter_pitcher_matchup_obp.csv: obp of all matchups

### General JSONs
train_val_test_indices.json: json file that contains the indices to use to create our training set, validation set, and test set

train_val_test_indices_with_2019.json: json file that contains the indices to use to create our training set, validation set, and test set for dataset that includes 2019 season

test_set_random.json: a test set that contains a pitcher id, batter id, the empirical matchup obp, and a string of the pitcher vs batter

test_set_chosen_obp_range.json: a test set by choosing pitchers with opposing obp between 0.295 and 0.3, choosing batters with obp in same range, then selecting all matchups between those batters and pitchers with the empirical obp of that matchup. An entry also exists with the average obp of all the matchups in the set. 


### Swing JSONs
swingTransition_allPitchers_newZones.json: old transition functions for all pitchers and rhh count unconditional

swingTransition_allPitchers_newZones_countConditional.json: old transition functions for all pitchers and rhh count conditional

swing_transition_all_pitchers.json: current transition functions for all pitchers and rhh count unconditional

swing_transition_all_pitchers_count_conditional.json: current transition functions for all pitchers and rhh count conditional


### Take JSONs
take_data_error_model.json: current pitcher error model to determine actual from intended location


## Zones
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

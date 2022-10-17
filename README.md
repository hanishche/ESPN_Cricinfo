# ESPN_Cricinfo


Scraping and Cleaning India T20's data by year Via Espn-cricinfo
This code provides 4 outputs namely Scoreboard , players_info , data_final (merge of scoreboard, players_info and impact score) and df_combined (concat of all above three files for an year)

You can get data of any team by updating the below line of code in Matches function:

url=requests.get("https://stats.espncricinfo.com/ci/engine/records/team/match_results.html?class=3;id={};team=6;type=year".format(year))

You can update team id "team=6" and get data accordingly


| Column| Description |
| --- | --- |
| age_days | Age of Player in days |
| age_years | Age of player in Years |
| keeper | Is player keeper? |
| known_as | Player_name |
| player_id | Unique Id of player |
| object_id | Unique Id of player in Espn website |
| player_primary_role | Role of Player (batsmen,allrounder,bowler) |
| popular_name | Name of player popularly known as |
| alpha_name | Name of player in short |
| batsmen | Boolean (1,0) |
| allrounder | Boolean (1,0) |
| bowler | Boolean (1,0) |
| BATTING | Scoreboard player name |
| CB | Caught & Bowled |
| R | Runs |
| B | Balls |
| M | Minutes |
| 4s | No of fours |
| 6s | No of sixes |
| SR | Strike rate |
| caught | Caught by |
| bowled | Bowled by |
| match_date | Date of match |
| team | Team name |
| recent_no_of_days | Today-Match date |
| run_out_1 | runout by |
| run_out_2 | run out assisted |
| stumped_out_by | stumped by |
| BOWLING | Bowler Name |
| Overs | No Of overs Bowled |
| Maidens | Maiden overs |
| Bowling_Runs | Runs_given by bowler |
| Wickets | Wickets Taken by bowler |
| ECON | Economy |
| Dots | Dot balls |
| fours | No of 4's |
| sixes | No of 6's |
| WD | Wide |
| NB | No ball |
| PLAYER | Player name in impact table |
| Team | Team of Player |
| TI | Total Impact points |
| Runs(Balls) | Runs of balls |
| I. Runs | Impact runs |
| Bowl | Bowling figures |
| I. Wkts | Impact wicket point |
| match_id | Id of the match |
| catch_by_substitute | Catch by substitute |
| lbw_by | lbw by |
| run_out_dh | run out direct hit |
| stumped_out_by | stumped_by |
| catch_by_substitute |	substitute_catch |



Note: *MVP (Impact score is only available from 2022 matches)

This notebook uses library created by @soodoku - https://github.com/outside-edge/python-espncricinfo/tree/e7968c696467491cc44d7f5b9fa99bb885cbce3c

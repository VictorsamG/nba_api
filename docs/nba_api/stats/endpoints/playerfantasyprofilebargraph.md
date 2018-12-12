# PlayerFantasyProfileBarGraph
##### [nba_api/stats/endpoints/playerfantasyprofilebargraph.py](https://github.com/swar/nba_api/blob/master/nba_api/stats/endpoints/playerfantasyprofilebargraph.py)

##### Endpoint URL
>[https://stats.nba.com/stats/playerfantasyprofilebargraph](https://stats.nba.com/stats/playerfantasyprofilebargraph)

##### Valid URL
>[https://stats.nba.com/stats/playerfantasyprofilebargraph?LeagueID=&PlayerID=2544&Season=2018-19&SeasonType=](https://stats.nba.com/stats/playerfantasyprofilebargraph?LeagueID=&PlayerID=2544&Season=2018-19&SeasonType=)

## Parameters
API Parameter Name | Python Parameter Class | Python Parameter Variable | Pattern | Required | Nullable
------------ | ------------ | ------------ | :-----------: | :---: | :---:
_**PlayerID**_ | [PlayerID](https://github.com/swar/nba_api/blob/master/docs/nba_api/stats/library/parameters.md#PlayerID) | player_id |  | `Y` |  | 
_**Season**_ | [Season](https://github.com/swar/nba_api/blob/master/docs/nba_api/stats/library/parameters.md#Season) | season | `^\d{4}-\d{2}$` | `Y` |  | 
_**SeasonType**_ | [SeasonTypeAllStarNullable](https://github.com/swar/nba_api/blob/master/docs/nba_api/stats/library/parameters.md#SeasonType) | season_type_all_star_nullable | `^(Regular Season)\|(Pre Season)\|(Playoffs)\|(All Star)$` |  | `Y` | 
_**LeagueID**_ | [LeagueIDNullable](https://github.com/swar/nba_api/blob/master/docs/nba_api/stats/library/parameters.md#LeagueID) | league_id_nullable | `(00)\|(20)\|(10)` |  | `Y` | 

## Data Sets
#### LastFiveGamesAvg `last_five_games_avg`
```text
['PLAYER_ID', 'PLAYER_NAME', 'TEAM_ID', 'TEAM_ABBREVIATION', 'FAN_DUEL_PTS', 'NBA_FANTASY_PTS', 'PTS', 'REB', 'AST', 'FG3M', 'FT_PCT', 'STL', 'BLK', 'TOV', 'FG_PCT']
```

#### SeasonAvg `season_avg`
```text
['PLAYER_ID', 'PLAYER_NAME', 'TEAM_ID', 'TEAM_ABBREVIATION', 'FAN_DUEL_PTS', 'NBA_FANTASY_PTS', 'PTS', 'REB', 'AST', 'FG3M', 'FT_PCT', 'STL', 'BLK', 'TOV', 'FG_PCT']
```


## JSON
```json
{
    "data_sets": {
        "LastFiveGamesAvg": [
            "PLAYER_ID",
            "PLAYER_NAME",
            "TEAM_ID",
            "TEAM_ABBREVIATION",
            "FAN_DUEL_PTS",
            "NBA_FANTASY_PTS",
            "PTS",
            "REB",
            "AST",
            "FG3M",
            "FT_PCT",
            "STL",
            "BLK",
            "TOV",
            "FG_PCT"
        ],
        "SeasonAvg": [
            "PLAYER_ID",
            "PLAYER_NAME",
            "TEAM_ID",
            "TEAM_ABBREVIATION",
            "FAN_DUEL_PTS",
            "NBA_FANTASY_PTS",
            "PTS",
            "REB",
            "AST",
            "FG3M",
            "FT_PCT",
            "STL",
            "BLK",
            "TOV",
            "FG_PCT"
        ]
    },
    "endpoint": "PlayerFantasyProfileBarGraph",
    "last_validated_date": "2018-12-11",
    "nullable_parameters": [
        "LeagueID",
        "SeasonType"
    ],
    "parameter_patterns": {
        "LeagueID": "(00)|(20)|(10)",
        "PlayerID": null,
        "Season": "^\\d{4}-\\d{2}$",
        "SeasonType": "^(Regular Season)|(Pre Season)|(Playoffs)|(All Star)$"
    },
    "parameters": [
        "LeagueID",
        "PlayerID",
        "Season",
        "SeasonType"
    ],
    "required_parameters": [
        "PlayerID",
        "Season"
    ],
    "status": "success"
}
```

Last validated 2018-12-11
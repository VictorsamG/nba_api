# FranchiseHistory
##### [nba_api/stats/endpoints/franchisehistory.py](https://github.com/swar/nba_api/blob/master/nba_api/stats/endpoints/franchisehistory.py)

##### Endpoint URL
>[https://stats.nba.com/stats/franchisehistory](https://stats.nba.com/stats/franchisehistory)

##### Valid URL
>[https://stats.nba.com/stats/franchisehistory?LeagueID=00](https://stats.nba.com/stats/franchisehistory?LeagueID=00)

## Parameters
API Parameter Name | Python Parameter Class | Python Parameter Variable | Pattern | Required | Nullable
------------ | ------------ | ------------ | :-----------: | :---: | :---:
_**LeagueID**_ | [LeagueID](https://github.com/swar/nba_api/blob/master/docs/nba_api/stats/library/parameters.md#LeagueID) | league_id | `^\d{2}$` | `Y` |  | 

## Data Sets
#### DefunctTeams `defunct_teams`
```text
['LEAGUE_ID', 'TEAM_ID', 'TEAM_CITY', 'TEAM_NAME', 'START_YEAR', 'END_YEAR', 'YEARS', 'GAMES', 'WINS', 'LOSSES', 'WIN_PCT', 'PO_APPEARANCES', 'DIV_TITLES', 'CONF_TITLES', 'LEAGUE_TITLES']
```

#### FranchiseHistory `franchise_history`
```text
['LEAGUE_ID', 'TEAM_ID', 'TEAM_CITY', 'TEAM_NAME', 'START_YEAR', 'END_YEAR', 'YEARS', 'GAMES', 'WINS', 'LOSSES', 'WIN_PCT', 'PO_APPEARANCES', 'DIV_TITLES', 'CONF_TITLES', 'LEAGUE_TITLES']
```


## JSON
```json
{
    "data_sets": {
        "DefunctTeams": [
            "LEAGUE_ID",
            "TEAM_ID",
            "TEAM_CITY",
            "TEAM_NAME",
            "START_YEAR",
            "END_YEAR",
            "YEARS",
            "GAMES",
            "WINS",
            "LOSSES",
            "WIN_PCT",
            "PO_APPEARANCES",
            "DIV_TITLES",
            "CONF_TITLES",
            "LEAGUE_TITLES"
        ],
        "FranchiseHistory": [
            "LEAGUE_ID",
            "TEAM_ID",
            "TEAM_CITY",
            "TEAM_NAME",
            "START_YEAR",
            "END_YEAR",
            "YEARS",
            "GAMES",
            "WINS",
            "LOSSES",
            "WIN_PCT",
            "PO_APPEARANCES",
            "DIV_TITLES",
            "CONF_TITLES",
            "LEAGUE_TITLES"
        ]
    },
    "endpoint": "FranchiseHistory",
    "last_validated_date": "2018-12-11",
    "nullable_parameters": [],
    "parameter_patterns": {
        "LeagueID": "^\\d{2}$"
    },
    "parameters": [
        "LeagueID"
    ],
    "required_parameters": [
        "LeagueID"
    ],
    "status": "success"
}
```

Last validated 2018-12-11
|Risk ID|Category|Risk Description        |Probability|Impact|Risk Score|Mitigation Strategy                                 |Indicator                   |Contingency Plan                        |Responsible|Status  |Last Modified Date|
|-------|--------|------------------------|-----------|------|----------|----------------------------------------------------|----------------------------|----------------------------------------|-----------|--------|------------------|
|1      |DB      |DB-Server is unavailable|<1%        |HIGH  |3 von 10  |Usage of HA and Fault Tolerance for better stability|no response                 |Transfer to new DB, via Transaction Logs|Manuel     |pending |11. Apr           |
|2      |Quality |Bugs in the software    |100%       |HIGH  |9 von 10  |Usage of Tests, Code Reviews                        |unexpected software behavior|Fix the issues                          |All        |pending |11. Apr           |
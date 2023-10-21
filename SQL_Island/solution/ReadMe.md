
**solution - SQL Island**

---

|  #    | meine Lösung                                                                                                                      |
| :---: | --------------------------------------------------------------------------------------------------------------------------------- |
| 1     | select * from bewohner                                                                                                            |
| 2     | select * from bewohner where status = "friedlich"                                                                                 |
| 3     | select * from bewohner where beruf = "Waffenschmied" and status = "friedlich"                                                     |
| 4     | select * from bewohner where beruf like "%schmied" and status = "friedlich"                                                       |
| 5     | select bewohnernr from bewohner where name = "Fremder"                                                                            |
| 6     | select gold from bewohner where bewohnernr = 20                                                                                   |
| 7     | select * from gegenstand where besitzer is null                                                                                   |
| 8     | update gegenstand set besitzer = 20 where besitzer is null                                                                        |
| 9     | select * from gegenstand where besitzer = 20                                                                                      |
| 10    | select * from bewohner where status = "friedlich" and (beruf = "Haendler" or beruf = "Kaufmann")                                  |
| 11    | update gegenstand set besitzer = 15 where gegenstand = "Ring" OR gegenstand = "Teekanne"                                          |
| 12    | update bewohner set name = "Woitschek" where bewohnernr = 20                                                                      |
| 13    | select * from bewohner where beruf = "Bäcker" order by name                                                                       |
| 14    | select * from bewohner where beruf = "Pilot"                                                                                      |
| 15    | select bewohner.name from bewohner, dorf where bewohner.bewohnernr = dorf.haeuptling and dorf.name = "Zwiebelhausen"              |
| 16    | select count(*) from bewohner, dorf where dorf.dorfnr = bewohner.dorfnr and dorf.name = 'Zwiebelhausen' and geschlecht = "w"      |
| 17    | select bewohner.name from bewohner, dorf where dorf.dorfnr = bewohner.dorfnr and dorf.name = 'Zwiebelhausen' and geschlecht = "w" |
| 18    | select sum(bewohner.gold) from bewohner where bewohner.beruf in ("Haendler", "Kaufmann", "Baecker")                               |
| 19    | select status, avg(bewohner.gold) from bewohner group by status order by avg(bewohner.gold)                                       |
| 20    | delete from bewohner where name = "Dirty Doerthe"                                                                                 |
| 21    | update bewohner set status = "friedlich" where beruf = "Pilot"                                                                    |

---

Zertifikat:

<img src="https://github.com/dr-woitschek/learn/blob/main/SQL_Island/solution/Certificate_SQL-Island.jpg" width="50%">

---

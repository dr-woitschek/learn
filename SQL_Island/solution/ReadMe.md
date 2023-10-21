
**solution - SQL Island**

---

|  #  | meine Lösung                                                                                                                      |
| --- | --------------------------------------------------------------------------------------------------------------------------------- |
| 1   | select * from bewohner                                                                                                            |
| 2   | select * from bewohner where status = "friedlich"                                                                                 |
| 3   | select * from bewohner where beruf = "waffenschmied" and status = "friedlich"                                                     |
| 4   | select * from bewohner where beruf like "%schmied" and status = "friedlich"                                                       |
| 5   | select bewohnernr from bewohner where name = "fremder"                                                                            |
| 6   | select gold from bewohner where bewohnernr = 20                                                                                   |
| 7   | select * from gegenstand where besitzer is null                                                                                   |
| 8   | select * from gegenstand where besitzer = 20                                                                                      |
| 9   | update gegenstand set besitzer = 20 where besitzer is null                                                                        |
| 10  | select * from gegenstand where besitzer = 20                                                                                      |
| 11  | select * from bewohner where status = "friedlich" and (beruf = "Haendler" or beruf = "Kaufmann")                                  |
| 12  | update gegenstand set besitzer = 15 where gegenstand = "Ring" OR gegenstand = "Teekanne"                                          |
| 13  | update bewohner set name = "Woitschek" where bewohnernr = 20                                                                      |
| 14  | select * from bewohner where beruf = "Bäcker" order by name                                                                       |
| 15  | select * from bewohner where beruf = "Pilot"                                                                                      |
| 16  | select bewohner.name from bewohner, dorf where bewohner.bewohnernr = dorf.haeuptling and dorf.name = "Zwiebelhausen"              |
| 17  | select count(*) from bewohner, dorf where dorf.dorfnr = bewohner.dorfnr and dorf.name = 'Zwiebelhausen' and geschlecht = "w"      |
| 18  | select bewohner.name from bewohner, dorf where dorf.dorfnr = bewohner.dorfnr and dorf.name = 'Zwiebelhausen' and geschlecht = "w" |
| 19  | select sum(bewohner.gold) from bewohner where bewohner.beruf in ("Haendler", "Kaufmann", "Baecker")                               |
| 20  | select status, avg(bewohner.gold) from bewohner group by status order by avg(bewohner.gold)                                       |
| 21  | delete from bewohner where name = 'Dirty Doerthe'                                                                                 |
| 22  | update bewohner set status = "friedlich" where beruf = "Pilot"                                                                    |

---

Zertifikat:

<img src="https://github.com/dr-woitschek/learn/blob/main/SQL_Island/solution/Certificate_SQL-Island.jpg" width="50%">

---

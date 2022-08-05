- [Dashboard](https://docs.google.com/spreadsheets/d/e/2PACX-1vSxAq359Zgp_kxZEiTV1zGVzYNmEJa5QKZRqCywPNf-lyOU6VzeVv5MzQKK6O10xFC8FB5y1MCM2RJD/pubhtml)
- [Spreadsheet](https://docs.google.com/spreadsheets/d/1RXLsHORnc2MLNxN2x8aK48RQ4ufn8h-1U-I43RrC9wA/edit#gid=126778419)
-
- ```mysql
  =QUERY(
    QUERY(Summary_Intermediate!F2:H, "select F, count(F)/"&count(Summary_Intermediate!B3:B200)&", min(G), avg(G), avg(H), max(G) where F is not null and G is not null and H is not null group by F order by count(F)/"&count(Summary_Intermediate!B3:B200)&" desc, min(G) desc, avg(G) desc label max(G) 'Max Size', min(G) 'Min Size', avg(G) 'Avg Size', avg(H) 'Avg Size % wrt team size', count(F)/"&count(Summary_Intermediate!B3:B200)&" '% of teams having division' format avg(G) '#.#', avg(H) '#.# %'"),
    "select * where Col1 != 'Autonomous Systems' and Col2>=0.2 format Col2 '#.# %'"
  )
  ```
	- `H is not null` will ensure that outlier team details (such as divisions in team sizes < 20) are exluded
	- `Col1 != 'Autonomous Systems'` eliminates Autonomous Systems from the dashboard because [[Sai]] said it's too complex for us
	- `Col2>0.2` tries to limit to the most important teams
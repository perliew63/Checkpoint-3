# Checkpoint-3
--Do NFL fans know more about who the best quarterbacks are?
```select
qb,
avg(game_points) as avg_points
from datasets.qbstats_1996_2016
group by qb
order by avg_points DESC

```
![Checkpoint#3](Picture1.png)

--rank the student from highest to lowest by sat_verbal?
```SELECT sat_verbal, student_id
 FROM datasets.sat_scores
 ORDER BY sat_verbal DESC
```
![ICA4_Perlie](satverbal.png)

--rank the students’ school from highest to lowest by hrs_studied
```SELECT school, hrs_studied
FROM datasets.sat_scores 
ORDER BY hrs_studied DESC
```
![ICA4_Perlie](hrs_studied.png)

--which students has the sat_writing scores over 600?
```SELECT student_id, sat_writing 
FROM datasets.sat_scores
WHERE sat_writing >600
ORDER BY sat_scores ASC 
```
![ICA4_Perlie](sat_writing.png)

--which students has the highst sat_verbal score?
```SELECT student_id, sat_verbal
FROM datasets.sat_scores
ORDER BY sat_verbal DESC
```
![ICA4_Perlie](sat_verbal_rank.png)

 1. Contare quanti iscritti ci sono ogni anno
 SELECT YEAR(`enrolment_date`) AS `anno`, COUNT(`id`) AS `tot iscritti per anno` 
 FROM `students` 
 GROUP BY YEAR(`enrolment_date`);
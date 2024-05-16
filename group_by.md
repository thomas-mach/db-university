 1. Contare quanti iscritti ci sono ogni anno
 SELECT YEAR(`enrolment_date`) AS `anno`, COUNT(`id`) AS `tot iscritti per anno` 
 FROM `students` 
 GROUP BY YEAR(`enrolment_date`);

 2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
 SELECT `office_address`, COUNT(*) AS `nr insenianti nel edificio` 
 FROM `teachers` 
 GROUP BY `office_address`;

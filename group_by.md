 1. Contare quanti iscritti ci sono ogni anno
 SELECT YEAR(`enrolment_date`) AS `anno`, COUNT(`id`) AS `tot iscritti per anno` 
 FROM `students` 
 GROUP BY YEAR(`enrolment_date`);

 2. Contare gli insegnanti che hanno l'ufficio nello stesso edificio
 SELECT `office_address`, COUNT(*) AS `nr insenianti nel edificio` 
 FROM `teachers` 
 GROUP BY `office_address`;

 3. Calcolare la media dei voti di ogni appello d'esame
 SELECT `exam_id`, AVG(`vote`) AS `media_voto` 
 FROM `exam_student` 
 GROUP BY `exam_id`;

 4. Contare quanti corsi di laurea ci sono per ogni dipartimento
 SELECT `department_id`, COUNT(*) AS `numero_di_corsi` 
 FROM `degrees` 
 GROUP BY `department_id`;


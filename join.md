1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia
SELECT DISTINCT CONCAT(`students`.`name`,' ',`students`.`surname`) AS `student_name` , `degrees`.`name` AS `cours_name` 
FROM `degrees` 
JOIN `courses` ON `courses`.`degree_id` = `degrees`.`id` 
JOIN `students` ON `students`.`degree_id` = `degrees`.`id` 
WHERE `degrees`.`name` = 'Corso di Laurea in Economia';
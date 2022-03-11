# verou-3-sql-introduction-benjaminlangenaken

* Get all data from the groups:

SELECT

      *
  FROM

    `groups`

<br>

* Get the name and email of the first learner, and alias the name to learner_name:

SELECT

    name as learner_name,
    email
FROM

    `learners`
WHERE

    id = 1

<br>

* Update the start date of the first_group (make it two months later):

UPDATE

    `groups`
SET

    start_date = start_date + INTERVAL 2 MONTH
WHERE

    id = 1

<br>

* One of the learners changed his/her mind and decided to be an astronaut:

DELETE FROM

    `learners`
WHERE

    id = 3
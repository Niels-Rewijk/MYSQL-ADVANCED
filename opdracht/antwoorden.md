# Antwoorden Eindopdracht

1. Copy paste je gemaakte SQL query hieronder
   SELECT `name`,`date` FROM `races` WHERE `year` = 2018
2. Copy paste je gemaakte SQL query hieronder
   SELECT drivers.surname, races.name, driver_standing.points FROM `drivers` LEFT JOIN driver_standing ON drivers.driverId = driver_standing.driverId LEFT JOIN races ON races.raceId = driver_standing.raceId WHERE races.year=2017 and driver_standing.points = 10
3. Copy paste je gemaakte SQL query hieronder
   SELECT drivers.forename, drivers.surname, pitstops.duration FROM `drivers` LEFT JOIN pitstops ON drivers.driverId = pitstops.driverId WHERE duration <= 25
4. Copy paste je gemaakte SQL query hieronder
   SELECT constructors.name, races.name, races.year FROM `constructors` LEFT JOIN constructor_standing ON constructor_standing.constructorId = constructors.constructorId LEFT JOIN races ON races.raceId = constructor_standing.raceId WHERE constructors.name = "McLaren" AND races.year = 2010
5. Copy paste je gemaakte SQL query hieronder
   SELECT circuits.name, circuits.country, drivers.surname, races.year FROM `circuits` LEFT JOIN races ON races.circuitId = circuits.circuitId LEFT JOIN driver_standing ON driver_standing.raceId = races.raceId LEFT JOIN drivers ON drivers.driverId = driver_standing.driverId WHERE races.year = 1950 and drivers.surname LIKE "f%"

# Antwoorden

1. Copy paste je gemaakte SQL query hieronder
   SELECT `name`, platform FROM game LEFT JOIN platform ON platform.id = game.platform_id WHERE game.name LIKE "Grand Theft Auto%"
2. Copy paste je gemaakte SQL query hieronder
   SELECT game.name FROM game RIGHT JOIN platform ON platform.id = game.platform_id WHERE platform.platform = "SCD"

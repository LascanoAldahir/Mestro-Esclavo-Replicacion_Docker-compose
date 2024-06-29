docker compose up -d <br> 
ESCLAVO <br>
SHOW MASTER STATUS el cual nos dará el File y Position <br>
CHANGE MASTER TO MASTER_HOST='MySQL_maestro', MASTER_USER='root',
MASTER_PASSWORD='root'; <br>

CHANGE MASTER TO MASTER_LOG_FILE='mysql-bin.000003', MASTER_LOG_POS=466; <br>
<br>
START SLAVE;
<br>
SHOW SLAVE STATUS;

<br>![image](https://github.com/LascanoAldahir/Replicacion_Docker-compose/assets/139184732/9006fe0e-b4db-4119-b6be-f8912ddfef5f)

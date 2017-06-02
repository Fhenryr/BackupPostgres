# BackupPostgres

#!/bin/bash

export PGPASSWORD="123456"


pg_dump -U postgres -h localhost -O -o -b -F c TesteSesc > /home/Marcelo/Documentos/TesteSesc_backup

echo echo "Backup OK."
exit 



---




#!/bin/bash

export PGPASSWORD="123123"

pg_restore -U postgres -h localhost -d TesteSesc1 /home/Marcelo/Documentos/TesteSesc_backup



echo echo "Backup restaurado."
exit 

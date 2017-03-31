# flyway-getting-started

> DOCUMENTAZIONE DA COMPLETARE

Questo repository contiene un esempio di applicazione delle fix. Per praticità utilizza sqlite come database. Questo repository è di fatto autoconsistente.

Istruzioni
-----------

1. Eseguire il clone del repository (``git clone https://github.com/wedoit-io/flyway-getting-started``)
2. Entrare nella directory flyway-getting-started (``cd flyway-getting-started``)
3. Verificare la lista delle fix da applicare (``flyway -configFile=conf/sample-client1.cfg info``)
4. Applicare le fix (``flyway -configFile=conf/sample-client1.cfg migrate``)
5. Verificare che le fix siano state applicate (``sqlite3 flyway-test.db "SELECT sql FROM sqlite_master"``)

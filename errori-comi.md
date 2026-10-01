Ho fatto il commit e poi trovo un refuso
Se ho appena fatto un commit e mi accorgo di un errore, posso modificare il file e usare:
git add .
git commit --amend
In questo modo correggo l'ultimo commit senza crearne uno nuovo.

Ho fatto git add troppo presto
Se ho aggiunto un file per errore, posso rimuoverlo con:
git restore --staged nomeFile
Il file non viene cancellato: semplicemente non sarà più pronto per il commit.

Ho modificato un file per errore
Se voglio annullare le modifiche non ancora salvate in un commit, posso usare:
git restore nome-file
Il file torna all'ultima versione presente nel commit.

Ho dimenticato di fare git pull
Se provo a fare git push e Git segnala che il repository remoto contiene modifiche che non ho, devo prima aggiornare il repository locale:
git pull
Dopo aver risolto eventuali conflitti e verificato le modifiche, posso eseguire:
git push
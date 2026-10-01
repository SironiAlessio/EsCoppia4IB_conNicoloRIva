ALESSIO SIRONI A
NICOLO' RIVA B
https://github.com/SironiAlessioEsCoppia4IB_conNicoloRIva.git

Domanda 1
Il repository sul computer è la copia locale del progetto mentre quello su Github è la copia online e remota del progetto. Se Github sparisse perderesti il repository remoto, ma il repository locale sul computer rimarrebbe intatto


Domanda 2 
Git rifiuta per non perdere le modifiche già presenti nel repository remoto: ti chiede di fare prima un git pull, così da unire le modifiche remote con quelle locali.


Previsione
Se B provasse a fare push senza aver fatto pull, Git 
rifiuterebbe il push perché il repository remoto contiene 
modifiche che B non ha ancora sul computer.

Domanda 3
Il conflitto è stato generato dalle modifiche diverse fatte da A e B sulla stessa parte del README. È stato poi risolto da chi ha eseguito il merge, modificando il file e scegliendo quale versione mantenere.
Se B avesse usato git push --force al punto 2, avrebbe sovrascritto la versione presente sul repository remoto, rischiando di cancellare le modifiche già pubblicate da A.

Domanda 4
Invertire i ruoli non avrebbe cambiato il modo di risolvere il conflitto, perché la procedura di merge rimane la stessa. Abbiamo verificato chi ha scritto cosa usando git log e git shortlog, che mostrano gli autori dei commit.
Con una Pull Request, il branch sarebbe stato prima revisionato dal compagno, che avrebbe potuto controllare le modifiche e segnalare eventuali problemi prima del merge
switch -c "branch" : crea un nuovo branch e entra dentro in questo
git merge "branch" : fa la merge del branch corrente con il branch indicato
fast-forward : git sposta il branch in avanti perché non ci sono modifiche concorrenti da unire
merge commit : git deve creare un nuovo commit che unisce due linee di sviluppo diverse
conflitto : nasce quando due branch modificano la stessa parte di un file e git non sa quale versione scegliere
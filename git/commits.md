# Rimuovere un commit su GitHub
Può capitare a tutti di eseguire un commit erroneamente, magari con un commento poco carino oppure con del codice incompleto, ma è facilmente risolvibile:

## Mantenere le modifiche in locale
Se il tuo obiettivo è solamente rimuovere il commit su github mantenendo le modifiche salvate nel tuo PC basta eseguire, dalla repository in questione, il seguente comando:
```bash
git reset --soft HEAD~1
```
Di seguito:
```bash
git push origin main --force
```
Oppure il nome del tuo branch al posto di `main`.

## Cancellare tutte le modifiche
Se invece vuoi "ripristinare" l'ultimo commit eliminando anche le modifiche fatte in locale basta eseguire:
```bash
git reset --hard HEAD~1
```
E poi:
```bash
git push origin main --force
```
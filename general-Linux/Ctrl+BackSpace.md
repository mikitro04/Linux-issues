# Configurare `Ctrl+BackSpace` su terminale Linux
Avete presente quando sbagliate a digitare una parola e per memoria muscolare premete `Ctrl + BackSpace` per cancellarla interamente?  
Se non sapete di cosa sto parlando benvenuti in una delle mie shortcut da tastiera preferite.

Se voleste farlo su un terminale Linux invece non farebbe niente, ma perchè?  
Perchè per il terminale la shortcut è `Alt + BackSpace`, ma siccome mi da abbastanza fastidio cambiare le mie abitudini ecco un modo per ovviare a questo problema mantenendo il classico `Ctrl + BackSpace`:

## Test
Per prima cosa verifichiamo che il sistema rilevi l'input in maniera corretta e distinta:  
Innanzi tutto premi su terminale `Ctrl + v` e `Ctrl + BackSpace`. Se il terminale ti restituisce `^H` allora possiamo passare alla fase due.

## Passo 2: Configura la tua shell 
Apri o crea tramite il tuo text editor preferito il file `~/.inputrc`, se non ne hai uno usa **nano**:
```bash
nano ~/.inputrc
```

Scrivi:
```bash
"\C-h": backward-kill-word
```

Salva con `Ctrl+O`, premi `Invio`, ed esci con `Ctrl+X`.

Infine ricarica le impostazioni digitando:
```bash
bind -f ~/.inputrc
```

## Conclusioni
That's all Folks!  
Alla prossima!
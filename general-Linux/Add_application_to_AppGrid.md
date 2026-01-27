# Aggiungere shortcut .desktop alla griglia delle applicazioni

## Cosa si intende per griglia delle applicazioni?

Se utilizzi **GNOME** come `Desktop Environment` premendo l'icona della tua distro ti apparirà una schermata in cui si possono vedere le tue applicazioni (sicuramente quelle di _snap_ oppure di _steam_).

Ma se installiamo un'applicazione tarmite `curl` oppure da un `tar.gz` può capitare che non siamo in grado di vederla.

<img width="1920" height="1080" alt="immagine" src="https://github.com/user-attachments/assets/f9761b76-934f-4e00-a6be-2e594782ed20" />

## Come fare?

Qua ti spiegherò come fare:

- Per prima cosa dovresti creare un collegamento a quella applicazione per accederci direttamente, per farlo l'ho spiegato in un altro file che puoi trovare [--> Qui](/general-Linux/Create_a_desktop_shortcut.md)
- Una volta creato il tuo collegamento quello che devi fare è spostarlo nella cartella `~/.local/share/applications`, puoi copiare di seguito il comando per farlo in automatico
  ```bash
  cp mio-file.desktop ~/.local/share/applications
  ```
 - Se non compare subito aspetta qualche istante

Tutto qua, più semplice di quanto si postesse immaginare

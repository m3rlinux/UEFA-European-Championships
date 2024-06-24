# UEFA European Championships

<a href="https://www.buymeacoffee.com/m3rlinux" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 30px !important;width: 108px !important;" ></a>

Visualizza il calendario e i risultati delle partite in tempo reale.

## Descrizione

L'applicazione si appoggia alle API Free [www.thesportsdb.com](https://www.thesportsdb.com/free_sports_api) e tramite una guida interattiva guida l'utente nella consultazione dei risultati delle partite.

## Getting started

### Installazione

L'eseguibile non ha bisogno di installazione e' sufficiente scaricarlo ed eseguirlo

### Configurazione

Alla prima esecuzione la guida interattiva chiede alcune info di base per la registrazione dell'utente, come

- nome utente
- e-mail (opzionale)

### Modificare il sorgente e ricreare l'eseguibile

Per poter modificare e testare i sorgenti occorre installare sul proprio sistema Python3 e Git, opzionale ma caldamente consigliato usare un IDE grafico, nel mio caso "IntelliJ IDEA".

**windows**

- [Python3](https://www.python.org/downloads/windows/) Consiglio di installare Python spuntando l'opzione "Add Python to PATH"
- [Git](https://gitforwindows.org/)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/download/?section=windows)

Dal menù "Start" selezionare "Git Bash" per aprire il prompt bash emulato.

Posizionarsi all'interno della cartella desiderata ed eseguire i seguenti comandi

``` bash
git clone https://github.com/m3rlinux/WorldCup2022.git
cd WorldCup2022
pip install pyinstaller
```

Abbiamo così clonato il progetto è installato il modulo pyinstaller che ci permettera di creare l'eseguibile.

Una volta effettuate le modifiche al sorgente eseguire il comando

``` bash
pyinstaller.exe --noconfirm --onefile --console --distpath "." --icon "src/uefa_euro.ico"  "src/uefa_euro.py"
```

### Licenza

Concesso in licenza secondo i termini della Licenza Apache, versione 2.0 [Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0).

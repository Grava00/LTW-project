# QuarantineHelp

Scopo del progetto: Il progetto nasce in un contensto di pandemia per aiutare la gente bisognosa a mettersi in contatto con volontari al fine di richiedere 
                    beni di prima necessità.

# Tecnologie utilizzate:
Sviluppo server (back-end):
Node.js, Express.js, Handlebars Template Engine, Bcrypt, Sequelize, PostgreSQL, ElephantSQL.
Sviluppo client: Bootstrap 4.0; JQuery; JavaScript; HTML5;

Api documentate: documentati con API Doc, /QuarantineHelp/Routes/docs/index.html,
Servizi REST: google maps, google calendar,
Servizi REST commerciali: google (passport), facebook (passport),
Servizio REST eseterno con OAuth: google calendar ,
Protocolli asincroni: Websocket per messaggisatica di assistenza con risposta statica e/o eventuale risposta via email

# Istruzioni installazione:

Una volta scaricata la cartella sarà necessario, da terminale, digitare "npm install" per installare tutte le dipendenze. 
Non sarà necessario scaricare alcun database, dal momento che l'app sfrutta un db condiviso (servizi Amazon).

# Istruzioni per il test:

Digitare "npm start" nella radice della cartella QuarantineHelp per avviare l'applicazione. Connettersi sul localhost alla porta 3000 tramite browser 
per visualizzare i contenuti.

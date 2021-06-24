# QuarantineHelp

Scopo del progetto: Il progetto nasce in un contensto di pandemia per aiutare la gente bisognosa a mettersi in contatto con volontari al fine di richiedere 
                    beni di prima necessità.

# Tecnologie utilizzate:
## Sviluppo server (back-end):
- Node.js
- Express.js
- Handlebars Template Engine
- Bcrypt
- Sequelize
- PostgreSQL
- ElephantSQL.

## Sviluppo client: 
- Bootstrap 4.0
- JQuery
- JavaScript
- HTML5


## API:
- documentati con API Doc, /QuarantineHelp/Routes/docs/index.html


### Servizi REST: 
- google maps
- google calendar
- SendGrid Mail

### Servizi REST commerciali
- google (passport)
- facebook (passport)

### Servizio REST eseterno con OAuth: 
- google calendar

### Protocolli asincroni: 

- Websocket per messaggisatica di assistenza con risposta statica e/o eventuale risposta via email

## Istruzioni installazione:

Una volta scaricata la cartella sarà necessario, da terminale, digitare "npm install" per installare tutte le dipendenze. 
Non sarà necessario scaricare alcun database, dal momento che l'app sfrutta un db condiviso (servizi Amazon).

# Istruzioni per il test:

Digitare "npm start" nella radice della cartella QuarantineHelp per avviare l'applicazione. Connettersi sul localhost alla porta 3000 tramite browser 
per visualizzare i contenuti. All'interno dell'applicazione sarà obbligatorio accedere/registrarsi per poter usufruire di tutte le funzionalità.
In particolare sarà obbligatorio scegliere un proprio ruolo all'interno della piattaforma (assistito/assistente) e sarà inoltre indispensabile rilasciare,
al momento della registrazione, un indirizzo di domicilio veritiero affinché si possa accedere. Ciò è controllato dalle API di Google (google maps).

Un assistito può accedere direttamente all'eshop, aggiungengere al carrello prodotti di cui necessita e inviare la sua richiesta a un volontario. La richiesta
verrà inviata al volontario più vicino (un algoritmo determinerà l'assistente più vicino in base agli utenti registrati come volontari nella città dell'assistito). 

Un assistente che riceve richieste le potrà vedere nel suo profilo, accettare o rifiutare. Una volta accettata potrà aggiungere al suo calendar l'evento i cui
dettagli sono: mittente della richiesta e beni richiesti, con timestamp della richiesta.
Se un assistente rifiuta una richiesta, questa viene inoltrata al secondo assisstene più vicino all'assistito, così fino a quando non finiscono i volontari
all'interno della città di domicilio dell'assistito.

Una richiesta inoltre può essere accettata e completata (una volta che il volontario ha soddisfatto la richiesta del proprio assistito).



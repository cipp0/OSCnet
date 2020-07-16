╔═╗╔═╗╔═╗┌┐┌┌─┐┌┬┐
║ ║╚═╗║  │││├┤  │
╚═╝╚═╝╚═╝┘└┘└─┘ ┴
#### Server per broadcasting di messaggi OSC via WAN diviso in gruppi
‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹‹

Progetto basato sulla libreria C++ OSCGroups di Ross Bencina

**Istruzioni per connettersi:**

- Avvia l’applicazione OSCnet.app
- Inserisci il tuo username
- Inserisci il nome del gruppo

**ATTENZIONE**
il nome del gruppo deve essere uguale per tutti i membri che vogliono partecipare alla sessione

**IMPORTANTE**
Né lo username né il nome del gruppo devono contenere spazi!

Una volta compilati i campi viene avviato un comando da terminale se viene riportato un messaggio con questa forma siamo connessi con successo al server:

```
ok: user ‘USERNAME’ is registered with server
ok: user ‘USERNAME’ is a member of group ‘NOMEGRUPPO’
user info received for ‘USERNAME’, private: il.mio.ip.privato:8087 public: il.mio.ip.pubblico:8087
```
Dove ```il.mio.ip.privato``` sta per la sequenza di numeri che compongono il mio IP privato della LAN e ```il.mio.ip.pubblico``` sta per la sequenza di numeri del mio IP Pubblico

**Istruzioni per mandare e ricevere messaggi OSC:**
- Apri una qualsiasi applicazione che ha implementato il protocollo OSC
(Ad esempio Max/MSP, PureData, CSound o SuperCollider)

- Invia i messaggi OSC all’indirizzo: localhost (oppure 127.0.0.1) alla porta 8087

- Ricevi i messaggi OSC da parte di tutti gli utenti collegati all’indirizzo:
localhost (oppure 127.0.0.1) alla porta 8089

Nel repository trovi una patch di esempio in Max/MSP 

Per disconnetterti dal server basta chiudere la shell del terminale

### Have fun!

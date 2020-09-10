![OSCnet01 logo](/oscnet01.png)
## ITA

#### Client per broadcasting di messaggi OSC via WAN diviso in gruppi (MacOS only)

Progetto basato sulla libreria C++ OSCGroups di Ross Bencina

**Istruzioni per connettersi al server di BitNet01:**

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

## ENG
#### Client for broadcasting of OSC messages via WAN divided into groups (MacOS only)

Project based on Ross Bencina's C ++ OSCGroups library

**Instructions to connect to the BitNet01 server:**

   - Start the OSCnet.app application
   - Enter your username
   - Enter the group name

**ATTENTION** 
the group name must be the same for all members who want to participate in the session

**IMPORTANT** 
Neither the username nor the group name must contain spaces!

Once the fields have been filled in, a command is started from the terminal if a message with this form is reported, we are successfully connected to the server:
```
ok: user 'USERNAME' is registered with server
ok: user 'USERNAME' is a member of group 'GROUPNAME'
user info received for 'USERNAME', private: my.private.IP: 8087 public: my.public.IP: 8087
```
Where ```my.private.IP``` stands for the sequence of numbers that make up my private LAN IP and ```my.public.IP``` stands for the sequence of numbers of my Public IP

**Instructions for sending and receiving OSC messages:**

- Open any application that has implemented the OSC protocol (For example Max / MSP, PureData, CSound or SuperCollider)
- Send OSC messages to the address: localhost (or 127.0.0.1) on port 8087
- Receive OSC messages from all users connected to the address: localhost (or 127.0.0.1) to port 8089

In the repository you find a sample patch in Max / MSP

To disconnect from the server just close the terminal shell

**Have fun!**

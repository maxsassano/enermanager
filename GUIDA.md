# 📖 Guida utente EnerManager

Manuale d'uso completo di EnerManager. Le stesse istruzioni sono disponibili nell'app al menu **Guida**.

---

## Indice

1. [Introduzione](#introduzione)
2. [Primo avvio e login](#primo-avvio-e-login)
3. [Impostazioni azienda](#impostazioni-azienda)
4. [Licenza e attivazione](#licenza-e-attivazione)
5. [Gestione utenti e permessi](#gestione-utenti-e-permessi)
6. [Clienti](#clienti)
7. [Cantieri](#cantieri)
8. [Operai](#operai)
9. [Rapportini](#rapportini)
10. [Impianti](#impianti)
11. [Mezzi](#mezzi)
12. [Manutenzioni e storico](#manutenzioni-e-storico)
13. [Magazzino](#magazzino)
14. [Calendario](#calendario)
15. [Report e PDF](#report-e-pdf)
16. [Inviare e condividere PDF](#inviare-e-condividere-pdf)
17. [Backup](#backup)
18. [Dove sono i dati](#dove-sono-i-dati)
19. [Supporto e contatti](#supporto-e-contatti)

---

## Introduzione

EnerManager è un'app per la gestione di cantieri, impianti e manutenzioni di una piccola azienda di elettricisti.

Include:

- Anagrafica clienti, operai, cantieri
- Rapportini giornalieri
- Impianti e manutenzioni programmate
- Mezzi aziendali e tagliandi
- Magazzino materiali
- Calendario appuntamenti
- Foto cantiere
- Stampa PDF di tutto
- Backup automatico

Tutti i dati sono salvati in un database locale sul tuo PC. **Nulla va online.**

---

## Primo avvio e login

Al primo avvio l'app crea automaticamente il database nella cartella `Documenti\EnerManager` e **un solo utente amministratore**:

- **admin / admin** (Titolare, vede tutto)

⚠️ **IMPORTANTE:** al primo accesso cambia subito la password di default!

Per creare altri utenti (amministrativo, operaio, ecc.) vai nel menu **Utenti** (visibile solo all'admin) e usa il pulsante **+ Nuovo utente**. Puoi assegnare a ciascuno i menu da vedere nella sidebar (checkbox) oppure usare i preset rapidi **Titolare**, **Amministrativo**, **Operaio**.

Spunta **Ricordami su questo PC** per non dover reinserire le credenziali ad ogni avvio.

Nella schermata di login trovi anche i contatti del supporto (helpdesk) in fondo.

---

## Impostazioni azienda

Dal menu **Impostazioni** (visibile solo a Titolare e Amministrativo) puoi inserire i dati della tua azienda:

- Nome, indirizzo, P.IVA, CF
- Telefono, email, sito
- Logo (PNG o JPG)

Questi dati appaiono nell'**intestazione di tutti i PDF** generati.

---

## Licenza e attivazione

EnerManager funziona in due modalità:

### Prova gratuita di 7 giorni
Parte automaticamente al primo avvio. Nel footer della sidebar vedi quanti giorni restano.

### Licenza attiva
Illimitata, sbloccata tramite seriale ricevuto dallo sviluppatore.

### Come attivare

1. Compila la **Partita IVA** in *Impostazioni* (serve per generare il seriale corretto)
2. Vai in **Impostazioni → sezione Licenza**
3. Incolla il seriale (formato `XXXXX-XXXXX-XXXXX-XXXXX`) e premi **Attiva EnerManager**

Se la prova è già scaduta, all'avvio appare la schermata **Prova scaduta** dove puoi inserire il seriale e attivare subito.

Per richiedere un seriale contatta lo sviluppatore: i contatti sono nella schermata di login e nella pagina **Informazioni**.

---

## Gestione utenti e permessi

Dal menu **Utenti** (solo Titolare) puoi:

- Creare nuovi utenti con password iniziale
- Modificare nome, ruolo, stato attivo/non attivo
- Scegliere quali menu della sidebar vede ogni utente (checkbox)
- Usare i preset rapidi: Titolare, Amministrativo, Operaio
- Reimpostare la password di un utente
- Eliminare utenti (tranne te stesso)

Il **ruolo** (Titolare, Amministrativo, Operaio) è puramente descrittivo. I permessi reali sono gestiti dalle checkbox menu.

Un utente vede nella sidebar solo le voci che gli sono state abilitate.

---

## Clienti

Dal menu **Clienti** puoi:

- Aggiungere un nuovo cliente con ragione sociale (aziende) o nome/cognome (privati)
- Inserire P.IVA, codice fiscale, indirizzo, contatti, note
- Cercare per nome, città, telefono
- Modificare o eliminare dalla lista
- Esportare la scheda cliente in PDF
- Inviare la scheda via email o condividerla

Toccando una riga si apre il **dettaglio cliente** con fatturato totale, cantieri e impianti.

---

## Cantieri

Dal menu **Cantieri** puoi:

- Creare un nuovo cantiere collegandolo a un cliente
- Specificare tipo (Fotovoltaico, Elettrico, ecc.), stato (In corso, Completato, ...)
- Impostare date di inizio/fine e importo preventivo
- Aggiungere **foto** dalla pagina Modifica cantiere (scatta o scegli da file)
- Modificare, eliminare o esportare la scheda PDF
- Inviare la scheda via email o condividerla

Toccando una riga si apre il **dettaglio cantiere** con spese, manodopera e rapportini.

---

## Operai

Dal menu **Operai** gestisci l'anagrafica del personale:

- Nome, cognome, mansione, costo orario
- Data nascita, data assunzione, contatti
- Stato attivo/non attivo
- Esportazione PDF scheda operaio con riepilogo ore annue
- Esportazione PDF **elenco completo** di tutti gli operai

---

## Rapportini

Il rapportino registra il lavoro fatto in cantiere per una data specifica.

**Passi:**

1. Menu Rapportini → **+ Nuovo rapportino**
2. Seleziona data e cantiere
3. Aggiungi gli operai con le ore lavorate
4. Aggiungi le voci (spese, materiali, vitto, benzina, alloggio, lavoro, trasferta)
5. Salva

Dal rapportino salvato puoi:
- Esportare il **PDF** con intestazione aziendale e firme
- Inviarlo via **email**
- **Condividerlo** con WhatsApp o altre app

---

## Impianti

Gli **impianti** sono i dispositivi installati dai tuoi clienti (caldaie, fotovoltaico, citofoni, cancelli, ecc.).

Per ogni impianto puoi impostare:

- Tipo e descrizione (voce libera)
- Cliente proprietario e ubicazione
- Periodicità manutenzione in mesi (es. 12)
- Ultima manutenzione e prossima scadenza (calcolata)

Puoi registrare **manutenzioni** fatte con costo, fornitore, esito e allegato PDF.

---

## Mezzi

I **mezzi** aziendali sono furgoni, auto, attrezzature.

Per ogni mezzo:

- Nome, targa, tipo
- Km attuali e intervallo tagliando
- Data e km ultimo tagliando

Puoi registrare i **tagliandi** fatti con costi e fornitore.

---

## Manutenzioni e storico

Il menu **Manutenzioni** mostra tutte le scadenze (impianti + mezzi) ordinate per urgenza.

**Filtri disponibili:** Tutte, Impianti, Mezzi, Scadute, Prossime 30 giorni.

Toccando una riga si apre direttamente l'impianto o il mezzo.

Il menu **Storico Manut.** mostra tutte le manutenzioni registrate con:
- Filtro per **anno**
- Filtro per **tipo** (impianti/mezzi)
- Ricerca per fornitore o descrizione
- **Totale del periodo**
- Export PDF della singola manutenzione

---

## Magazzino

Il **magazzino** tiene traccia delle giacenze materiali.

Per ogni materiale:

- Nome, categoria, unità di misura
- Quantità disponibile, costo unitario
- Fornitore, soglia di riordino

Con i pulsanti **+ Carico** e **- Scarico** registri i movimenti. La giacenza si aggiorna da sola.

Se un materiale scende sotto la soglia appare un **avviso rosso** in cima.

Puoi esportare il PDF del magazzino completo con totale valore e lista sotto scorta.

---

## Calendario

Il calendario mostra una griglia mensile con gli appuntamenti.

- Scegli **Mese** e **Anno** dai menu in alto
- I giorni con appuntamenti hanno un **pallino ambra**
- Clicca un giorno per vedere gli appuntamenti o aggiungerne uno

**Tipi disponibili:** Sopralluogo, Lavoro, Manutenzione, Consegna, Preventivo, Altro (ognuno con colore diverso).

Puoi collegare un appuntamento a un **cliente** e/o a un **cantiere**.

Toccando un appuntamento si apre il cantiere o il cliente collegato.

Puoi esportare il **PDF del mese** o dell'**anno** corrente.

---

## Report e PDF

Il menu **Report** genera report aggregati per **cantiere, cliente o operaio** nel periodo scelto.

- Scegli **Dal / Al** con i due date picker
- Scegli il **Filtro** tra Cantieri / Clienti / Operai
- Il report si aggiorna automaticamente al cambio di data o filtro
- Puoi esportarlo in **PDF** o inviarlo via **email**

Praticamente ogni elemento dell'app ha un pulsante PDF:

- Scheda cliente / cantiere / operaio / impianto / mezzo / manutenzione / materiale
- Magazzino completo
- Rapportino
- Report periodico
- Manuale utente
- Calendario mese/anno
- Elenco completo operai

Tutti i PDF hanno **intestazione aziendale con logo** e si aprono automaticamente.

---

## Inviare e condividere PDF

Su ogni elemento con PDF hai 3 opzioni:

1. **Pulsante PDF** → apre il PDF nel visualizzatore
2. **Pulsante Email** (verde) → apre il client email con allegato e oggetto precompilato
3. **Pulsante Share** (blu) → apre il pannello di condivisione di sistema

Su **Windows**, Share apre il menu Condividi di Windows.
Su **Android**, Share mostra WhatsApp, Telegram, Gmail, Drive, ecc.

Dalla condivisione puoi inviare il PDF via WhatsApp a un cliente o collega.

---

## Backup

Il menu **Backup** crea una copia di sicurezza di database e PDF in un unico file **ZIP** datato.

Consigliamo di fare un backup **ogni settimana** e di copiarlo su una chiavetta USB o su un servizio cloud (Google Drive, OneDrive).

I backup sono salvati in `Documenti\EnerManager\Backup`.

---

## Dove sono i dati

**Dove sono i miei dati?**
In `Documenti\EnerManager\` nel tuo profilo utente. Il file si chiama `enermanager.db3`.

**Come faccio un backup manuale?**
Copia il file `enermanager.db3` su una chiavetta USB.

**Posso usare l'app su un altro PC?**
Sì, installa EnerManager, poi copia il file `enermanager.db3` nella cartella `Documenti\EnerManager` del nuovo PC.

**Ho perso la password?**
Contatta l'amministratore (Titolare). Può reimpostarla dalla pagina Utenti.

**Il PDF non si apre?**
Controlla che ci sia un programma predefinito per aprire i PDF (Edge, Adobe Reader, ecc.).

**Ho bisogno di aiuto?**
Contatta lo sviluppatore: i contatti sono nella schermata di login e in Informazioni.

---

## Supporto e contatti

Nella **schermata di login** e nella pagina **Informazioni** trovi i contatti dello sviluppatore:

- **Email** → apre il client email
- **Telefono** → apre il dialer
- **Sito web** → apre il browser

Usali per:
- Richiedere un **seriale di attivazione**
- Segnalare un **problema**
- Chiedere **assistenza**

Nel footer della sidebar vedi sempre il tuo nome utente e lo stato della licenza (**ATTIVATO** verde / **Prova** in ambra).

---

© 2026 Massimo Sassano — Tutti i diritti riservati.

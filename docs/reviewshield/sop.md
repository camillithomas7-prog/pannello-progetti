# SOP — ReviewShield

> Procedure operative dal lead alla rimozione e all'incasso.
> Target: chirurghi plastici, medici estetici, dermatologi, cliniche.
> Modello: il cliente paga **solo dopo** che la recensione è sparita dal profilo.

---

## Indice

1. [Ruoli](#ruoli)
2. [SOP-01 — Lead in arrivo dalla dashboard](#sop-01--lead-in-arrivo-dalla-dashboard)
3. [SOP-02 — Pre-qualifica del profilo Google](#sop-02--pre-qualifica-del-profilo-google)
4. [SOP-03 — Primo contatto (telefono / WhatsApp)](#sop-03--primo-contatto-telefono--whatsapp)
5. [SOP-04 — Demo / Chiamata di vendita](#sop-04--demo--chiamata-di-vendita)
6. [SOP-05 — Chiusura e invio link Stripe](#sop-05--chiusura-e-invio-link-stripe)
7. [SOP-06 — Passaggio al team operativo](#sop-06--passaggio-al-team-operativo)
8. [SOP-07 — Lavorazione e aggiornamenti al cliente](#sop-07--lavorazione-e-aggiornamenti-al-cliente)
9. [SOP-08 — Conferma rimozione + incasso](#sop-08--conferma-rimozione--incasso)
10. [SOP-09 — Upsell post-vendita](#sop-09--upsell-post-vendita)
11. [SOP-10 — Casi limite e contestazioni](#sop-10--casi-limite-e-contestazioni)
12. [Numeri ufficiali da citare](#numeri-ufficiali-da-citare)

---

## Ruoli

| Ruolo | Chi | Cosa fa |
|---|---|---|
| **Owner** | Samuele + Thomas | Coordina, riceve incassi via Stripe, non parla coi clienti |
| **Venditore** | Closer esterno | Tutto il flusso commerciale: contatto → demo → chiusura → invio Stripe |
| **Team Analisti / Legale** | Operatori | Costruiscono il dossier e segnalano a Google |
| **Account Manager** | Operatore dedicato | Aggiorna il cliente ogni 48h, gestisce conferme rimozione |

> Sam e Thomas **non parlano coi clienti**. I venditori vendono, gli operatori rimuovono, il pagamento Stripe arriva sul conto.

---

## SOP-01 — Lead in arrivo dalla dashboard

**Fonte lead**: `https://reviewshieldita.lovable.app/admin/dashboard` (lead già scrapati: medici / chirurghi plastici / cliniche).

**Procedura**:
1. Venditore accede alla dashboard ogni mattina alle 9:00.
2. Filtra i lead per priorità:
   - **Priorità ALTA**: rating Google tra **3.5 e 4.3** (zona dove ogni recensione negativa pesa di più sulla scelta del paziente).
   - **Priorità MEDIA**: rating tra 4.4 e 4.6 con almeno 3 recensioni 1-2 stelle.
   - **Priorità BASSA**: rating ≥ 4.7 (poco margine, ma utile per Monitoraggio Continuo).
3. Assegna a sé stesso un blocco di 10–15 lead/giorno, marca lo stato a "in lavorazione".
4. Per ogni lead: passa a **SOP-02**.

**Tempistica**: ogni lead dev'essere contattato entro **48 ore** dall'assegnazione.

---

## SOP-02 — Pre-qualifica del profilo Google

**Da fare prima di chiamare**, ogni volta. Tempo richiesto: 5–7 minuti per profilo.

1. Apri il profilo Google del medico (Google Maps o Search).
2. Conta le recensioni 1 e 2 stelle degli ultimi 12 mesi.
3. Per ogni recensione negativa, classifica:
   - **Prematura** → scritta a giorni/settimane da un intervento che dà risultato a mesi.
   - **Dati medici esposti** → cita interventi, complicazioni, condizioni → violazione privacy.
   - **Diffamatoria** → "truffatore", "incompetente", "mi ha rovinato".
   - **Sospetta competitor** → account creato di recente, una sola recensione, profilo vuoto.
   - **Aspettativa irrealistica** → "volevo il naso di Belen", lavoro tecnicamente perfetto.
   - **Altro / non rimovibile** → critiche generiche e fondate.
4. Calcola il **danno stimato** (formula sotto).
5. Scegli 2–3 recensioni "facili" da mostrare in chiamata come esempio concreto.
6. Salva tutto in una nota interna sul lead nella dashboard.

**Formula danno (da usare in chiamata)**:
```
Pazienti persi/mese (stima) × Valore medio paziente × 12 = Danno annuo
```
Esempio chirurgo plastico:
- 2 pazienti persi/mese × 5.000 € = **10.000 €/mese persi**
- → 120.000 €/anno → **600.000 € in 5 anni**

Esempio medico estetico:
- 4 pazienti/mese × 800 € = **3.200 €/mese persi** → 38.400 €/anno

> Questa è l'arma principale di vendita. Il prezzo (€300/recensione) sembra niente confrontato al danno.

---

## SOP-03 — Primo contatto (telefono / WhatsApp)

**Canale preferito**: telefono diretto allo studio.
**Orari migliori**: martedì-giovedì, 10:00–12:00 e 15:00–17:00.

**Apertura standard** (15 secondi):
> "Buongiorno, sono [nome] di ReviewShield. Mi sono permesso di chiamare perché ho appena guardato il profilo Google del Dr. [Cognome] e ho visto che ci sono recensioni che secondo le policy Google sono rimovibili. Posso parlargli 2 minuti o richiamare in un altro momento?"

**Se non passa la segretaria**:
> "Ho letto le recensioni del dottore e ne ho identificate 3 che possono essere rimosse legalmente da Google. Lo dica al dottore, le lascio il mio numero — sono [nome], +39 XXX. La richiamata è gratuita e di interesse del dottore."

**Se risponde direttamente il medico**: vai a **SOP-04**.

**Se WhatsApp** (script completo in [`script-vendita.md`](script-vendita.md)):
> "Buongiorno Dr. [Cognome], sono [nome] di ReviewShield. Abbiamo analizzato il suo profilo Google e crediamo di poter rimuovere [X] recensioni negative. Le mando l'analisi gratuita? Le bastano 2 minuti per leggerla."

---

## SOP-04 — Demo / Chiamata di vendita

Durata target: **15–20 minuti**.

Struttura (dettaglio scriptato in [`script-vendita.md`](script-vendita.md)):

1. **Empatia** (2 min) — riconosci il dolore: "Quanto le pesa quella recensione?"
2. **Calcolo del danno** (3 min) — usa la formula di SOP-02. Il prezzo dopo questo step sembra ridicolo.
3. **Soluzione** (5 min) — chi siamo, come funziona:
   - Team analisti + team legale + account manager dedicato
   - 88% successo, 10 giorni medi (alcune in 48h)
   - 900+ recensioni eliminate, 200+ cliniche, 7 anni di attività
   - 5 policy Google sfruttate
   - 0 accessi al profilo, 0 credenziali richieste
4. **Garanzia** (1 min) — la frase chiave da ripetere:
   > **"Lei paga SOLO dopo che la recensione è sparita. Se non riusciamo, costo zero. Il rischio è tutto nostro."**
5. **Prezzi** (3 min) — vai a SOP-05.
6. **Chiusura** (2 min) — invio link Stripe.

**Mostrare in chiamata** (link / screenshot da mandare via WhatsApp durante la call):
- Case study Bologna: 9 recensioni rimosse, rating 3.6 → 4.7 in 12 giorni.
- Case study Milano: recensione di 2 anni, rimossa in 6 giorni.

---

## SOP-05 — Chiusura e invio link Stripe

**Listino ufficiale**:

| Pacchetto | Prezzo | Quando proporlo |
|---|---|---|
| **Pulizia Singola** | €300 / recensione | 1–3 recensioni da rimuovere |
| **Pacchetto 10** | €240 / recensione (sconto 20%) | 4+ recensioni |
| **Monitoraggio Continuo** | €100 / mese | Sempre, come upsell o per profili "sani" che vogliono prevenzione |

**Procedura invio link Stripe**:
1. Venditore chiede: nome esatto attività + URL profilo Google + email + WhatsApp.
2. Venditore richiede al team Sam/Thomas il **link Stripe corretto**:
   - One-shot per Pulizia (singola o pacchetto)
   - Subscription mensile per Monitoraggio
3. Sam/Thomas generano il link e lo girano al venditore.
4. Venditore inoltra al cliente via WhatsApp + email con questo testo:
   > "Dottore, come da accordo le mando il link Stripe. **Non lo paghi adesso** — apriamo il caso, rimuoviamo le recensioni, e quando le vede sparite saldano il link. Se non riusciamo, il link non viene mai pagato. Ci siamo?"
5. Venditore aggiorna lo stato del lead in dashboard: "Stripe inviato — in attesa rimozione".

**REGOLA FERREA**: il cliente **non paga prima della rimozione**. Mai. È il nostro principale argomento di vendita, non si tradisce.

---

## SOP-06 — Passaggio al team operativo

Una volta accettato l'accordo e inviato lo Stripe, il venditore prepara il **brief operativo**:

**Template brief** (da inviare via email o canale interno al team):
```
NUOVO CASO — ReviewShield

Cliente: Dr. [Nome Cognome]
Attività: [Nome esatto attività]
URL Google: [link profilo]
Città: [città]
Email: [email]
WhatsApp: [+39 ...]

Recensioni da rimuovere ([N] totali):
1. [URL recensione] — Autore: [nome] — Motivo: [policy violata] — Screenshot: [link]
2. ...

Pacchetto venduto: [Singola / Pacchetto 10 / Monitoraggio]
Importo: € [totale]
Stripe link: [URL] — stato: inviato, NON pagato

Note venditore: [contesto utile, sensibilità, urgenze]
```

Il team operativo prende in carico entro **24 ore** e contatta il cliente con un'email di benvenuto firmata dall'account manager.

---

## SOP-07 — Lavorazione e aggiornamenti al cliente

**Tempistica standard**: 10 giorni lavorativi (alcune recensioni cadono in 48h).

**Checkpoint obbligatori**:
- **Giorno 0**: email di benvenuto dell'account manager con timeline prevista.
- **Giorno 2**: aggiornamento "abbiamo costruito il dossier per recensioni X, Y, Z e abbiamo segnalato".
- **Giorno 5**: aggiornamento di stato (anche se "ancora in lavorazione").
- **Giorno 10**: aggiornamento finale — quante rimosse, quante in lavorazione, quante non eliminabili.

**Tono da usare** con il cliente: professionale, pacato, mai trionfalistico finché la recensione non è sparita. Quando è sparita: screenshot prima/dopo come prova.

**Se il caso supera i 14 giorni**: l'account manager fa una telefonata per spiegare lo stato senza far sentire il cliente abbandonato.

---

## SOP-08 — Conferma rimozione + incasso

Quando una recensione sparisce dal profilo Google:

1. Account manager verifica con due controlli a 24h di distanza (per essere sicuri che non sia un cache).
2. Salva screenshot **prima** (preso al momento della vendita) e **dopo**.
3. Invia email al cliente:
   > "Dottore, come promesso. La recensione di [autore] del [data] è stata rimossa definitivamente da Google. Le allego lo screenshot prima/dopo come prova.
   >
   > Come da accordo iniziale, può ora completare il pagamento del link Stripe che le abbiamo inviato il [data invio]. Se ha problemi col link, mi scriva.
   >
   > La ringraziamo della fiducia."
4. Notifica Sam/Thomas via canale interno: "Cliente X — rimossa, sollecitato pagamento Stripe".
5. Sam/Thomas controllano lo Stripe entro 48h. Se non pagato → SOP-10.

**Se subscription Monitoraggio**: il primo addebito parte dal mese successivo alla prima rimozione confermata.

---

## SOP-09 — Upsell post-vendita

**A 7 giorni dalla rimozione**, l'account manager propone:
- Se il cliente ha pagato singole → proporre **Pacchetto 10** scontato per recensioni future.
- Se il cliente non ha Monitoraggio → proporre **Monitoraggio Continuo €100/mese** con questo angolo:
  > "Dottore, oggi lei è pulito. Ma il problema può ripresentarsi: bastano 1–2 recensioni nuove e siamo punto a capo. Con il Monitoraggio le copriamo TUTTE le recensioni future automaticamente, lei non deve nemmeno chiamare. 100 euro al mese e dorme tranquillo."

**KPI minimo upsell**: il 30% dei clienti pulizia singola deve attivare Monitoraggio entro 30 giorni dalla prima rimozione.

---

## SOP-10 — Casi limite e contestazioni

### Caso A — Cliente non paga lo Stripe dopo rimozione
1. Account manager invia 1° sollecito (giorno +3): "Le ricordo gentilmente il link Stripe ancora aperto."
2. Account manager invia 2° sollecito (giorno +7): tono fermo ma cortese.
3. Sam/Thomas inviano sollecito formale (giorno +14): via PEC se disponibile, altrimenti email registrata.
4. Se non paga entro 30 giorni: passaggio a recupero crediti.

> Nota: nella nostra storia il tasso di insolvenza è bassissimo perché il cliente ha visto risultato concreto. Ma serve il processo.

### Caso B — Recensione rimossa che riappare
- La rimuoviamo **gratis**, è dichiarato sulla landing.
- Apri nuovo dossier, segnala nuovamente, comunica al cliente: "ce ne occupiamo noi senza costi aggiuntivi".

### Caso C — Recensioni che non riusciamo a rimuovere
- Comunica al cliente con onestà: "questa rientra nelle critiche fondate, Google non la rimuoverà. Possiamo lavorare sulle altre N che invece sono rimovibili."
- Costo per quelle non rimosse: **zero**, come da accordo.

### Caso D — Cliente vuole indietro i soldi dopo aver pagato
- Il pagamento Stripe è dovuto in cambio del risultato già consegnato (recensione rimossa).
- Mostrare screenshot prima/dopo, contratto/email di conferma.
- In caso di chargeback: contestare con la documentazione.

### Caso E — Recensione che il cliente ritiene rimovibile, ma non lo è
- Fai un'analisi onesta in fase di vendita: meglio dirlo prima che dopo.
- Se ti accorgi solo dopo: comunica al cliente, non addebitare nulla per quella, lavora solo su quelle effettivamente rimovibili.

---

## Numeri ufficiali da citare

Da memorizzare e ripetere SEMPRE in chiamata. Sono i numeri della landing, non si inventano.

| Metrica | Valore |
|---|---|
| Tasso di successo | **88%** |
| Recensioni eliminate (totale storico) | **900+** |
| Cliniche e studi serviti | **200+** |
| Tempo medio di rimozione | **10 giorni** lavorativi (alcune in 48h) |
| Anni di attività nel settore | **7 anni** |
| Anni esperienza team legale | **12+ anni** |
| Risposta entro | **2 ore** |
| Policy Google sfruttate | **5** (Contenuto Fuorviante, Privacy, Conflitto di Interessi, Diffamazione, Spam) |

**Trust badges (da ripetere a chiusura)**:
- ✅ Paghi solo dopo la rimozione
- ✅ Zero pagamenti anticipati
- ✅ 100% legale e conforme
- ✅ Nessun accesso al profilo

---

*Ultima revisione: vedi git log. Dubbi o aggiornamenti: parlare con Samuele o Thomas.*

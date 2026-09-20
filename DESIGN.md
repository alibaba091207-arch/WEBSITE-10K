# Design package: Bottega del Web

Tier 1, un solo video da 6 secondi scrubbato dallo scroll. Questo documento è l'input della build. Ogni riga di copy qui dentro va nel sito parola per parola.

## 1. La premessa del marchio

**La prova è davanti ai tuoi occhi.**

Tutte le agenzie dicono di fare bei siti. Noi non lo diciamo, lo facciamo vedere: il sito che stai guardando è la dimostrazione, e il tuo lo vedi finito prima di pagare qualcosa. Ogni sezione serve questa idea. Se una sezione non la serve, si taglia.

## 2. La palette

Presa dal mondo del video: vetro, acciaio, luce fredda nel buio.

```css
:root{
  --canvas:#0A0D14;        /* grafite inchiostro, mai nero puro */
  --panel:#121724;         /* superfici rialzate */
  --accent:#5EE3F5;        /* luce sul bordo del vetro. CTA e rara enfasi */
  --accent-hover:#93EEFA;
  --accent-muted:#1B4552;  /* bordi e particelle a sussurro */
  --text-primary:#EAF2F7;
  --text-secondary:#8A9AAB;
}
```

L'accento compare solo sulla CTA, sul focus da tastiera e su uno o due punti di enfasi per schermata.

## 3. Il trio di font

- **Display: Bricolage Grotesque** (700, 800). Solo dai 34px in su.
- **Testo: Schibsted Grotesk** (400, 500, 600). Cifre tabulari per i prezzi.
- **Etichette piccole: DM Mono** (400, 500). Numeri dei passi, micro etichette, righe tecniche.

## 4. L'elemento firma

**Il bordo di luce.** Una linea sottile ciano che si accende lungo un solo lato delle superfici chiave quando il pannello si incastra al suo posto, e i divisori di sezione che si disegnano da soli come fili di luce. Eco diretta del video. Tutto il resto della pagina resta silenzioso perché questa firma si legga.

## 5. La mappa delle bande

| Banda | Range | Momento del video | Copy | Entrata |
|---|---|---|---|---|
| 1 | 0.00 a 0.16 | il primo pannello sospeso, gli altri entrano | "Questo è il livello." | grid snap-align, i caratteri si allineano come lastre |
| 2 | 0.20 a 0.40 | i pannelli scendono e si impilano | "Il tuo sito può essere così." | drift-down, le parole scendono coi pannelli |
| 3 | 0.45 a 0.66 | la struttura si chiude e mette a fuoco | "E lo vedi finito prima di pagare." | blur-to-sharp, la messa a fuoco arriva |
| 4 | 0.72 a 1.00 | tutto fermo, la lastra riflette | "Zero euro finché non ti piace." | rise scaglionato: titolo, sottotitolo, bottone |

Banda 4, sottotitolo: "Realizzazione gratuita, poi 150 euro al mese con tutto incluso."
Banda 4, bottone: "Guarda il tuo sito"

I range sono punti di partenza, validati dopo col flick test.

## 6. L'eroe statico (telefoni e movimento ridotto)

- Titolo: "Il tuo sito può essere così."
- Sottotitolo: "Lo vedi finito prima di pagare. Se non ti piace, non paghi niente."
- Bottone: "Guarda il tuo sito"

## 7. Le sezioni sotto

Tutte portano a una sola azione: richiedere la demo gratuita su WhatsApp.

1. **I due preventivi.** Il conto dell'agenzia contro il nostro, solo numeri allineati. Agenzia: realizzazione 1.200 €, canone 150 €, modifiche a pagamento, primo anno 3.000 €. Noi: realizzazione 0 €, dominio più primo mese 179 €, canone 150 €, modifiche incluse, primo anno 1.979 €. Sopra la tabella, una riga: "In Italia un sito per una piccola attività costa in media tra 1.200 e 2.500 euro. Ecco il confronto, senza girarci intorno."

2. **Come funziona.** Tre passi numerati in DM Mono.
   1. "Ci racconti chi sei." / "Quindici minuti su WhatsApp. Ci basta per capire cosa fai."
   2. "Costruiamo il sito e te lo mostriamo." / "Finito, sul tuo telefono, coi tuoi testi veri. Prima che tu paghi qualcosa."
   3. "Se ti piace, andiamo online." / "Dominio, hosting, sicurezza, tutto incluso. Se non ti piace, non hai speso niente."

3. **Il momento interattivo: componi il tuo sito.** Tieni premuto e i pannelli si incastrano uno alla volta fino a formare una pagina finita. Lasci prima e tornano indietro piano. Completato, la sezione si accende in sequenza e appare la riga: "Ecco. Adesso fallo col tuo." Movimento ridotto: stato finale subito, senza tenere premuto.

4. **Pacchetti.** Tre blocchi, il primo col bordo acceso.
   - "Sito statico" / "Realizzazione gratuita · 150 €/mese" / "Te lo facciamo vedere finito. Se ti piace partiamo, se non ti piace non paghi niente." / bottone "Richiedi la demo gratuita"
   - "Sito su misura" / "Realizzazione da 899 € · 250 €/mese" / "Video, animazioni, costruito pezzo per pezzo sulla tua attività. Come questo che stai guardando." / bottone "Parliamone"
   - "Automazioni" / "Preventivo su misura" / "Un chatbot che risponde anche di notte, o il lavoro ripetitivo che si fa da solo." / bottone "Contattaci"

5. **Cosa c'è dentro.** Elenco con filo di luce tra le voci, scritto contro i costi nascosti trovati nella ricerca.
   - "Dominio registrato a tuo nome"
   - "Hosting e certificato di sicurezza"
   - "Modifiche ai testi incluse, quante ne vuoi"
   - "Backup automatico"
   - "Assistenza su WhatsApp, rispondiamo noi"
   - "Nessun costo a sorpresa. Quello che leggi è quello che paghi."

6. **Domande.** Le obiezioni vere trovate nella ricerca.
   - "Il dominio è mio?" / "Sì, registrato a tuo nome dal primo giorno. Resta tuo anche se un domani cambi fornitore."
   - "Cosa succede se smetto?" / "Il sito resta online fino alla fine del mese già pagato. Il dominio è tuo e te lo porti dove vuoi."
   - "Quanto ci vuole?" / "Lo vedi pronto in pochi giorni. Va online lo stesso giorno in cui ci dici di sì."
   - "Posso cambiare i testi da solo?" / "Scrivi su WhatsApp cosa cambiare e lo facciamo noi, incluso nel canone. Niente fatture per due righe di testo."
   - "Ho già Facebook e Instagram, mi serve un sito?" / "I social sono in affitto. La pagina può sparire domani per una segnalazione sbagliata. Il sito e il dominio sono tuoi, e su Google ci finisci solo con quelli."
   - "E se poi sparite?" / "Rispondiamo su WhatsApp, lo stesso numero che vedi qui sotto. E il dominio è a tuo nome, quindi non sei mai in ostaggio."

7. **Contatti.** Quattro campi: nome, numero WhatsApp, che attività hai, hai già un sito (No / Sì ma va rifatto / Sì e funziona bene). Bottone "Invia su WhatsApp". Nessun backend: al submit costruisce il link wa.me con i dati dentro e apre WhatsApp al numero +39 351 305 1629. Stato di successo: "Apriamo WhatsApp con il messaggio già scritto. Premi invio e ti rispondiamo."

8. **Footer.** Nome, numero WhatsApp, anno. Niente disclosure di marchio inventato: l'agenzia è vera. Le immagini generate restano senza dichiarazione, si sostituiranno con lavori veri.

## 8. Il livello vettoriale

- Divisori di sezione come fili di luce che si disegnano da soli allo scroll.
- Bordo di luce che si accende sul lato sinistro delle superfici chiave quando entrano.
- Particelle di polvere a sussurro nel livello di fondo fisso, ciclo da 60 secondi o più.
- Griglia di riferimento appena percepibile dietro la sezione interattiva, che richiama i pannelli del video.
- Tutto rispetta il movimento ridotto: stato finale mostrato, motori fermi.

## 9. L'ingegneria

Blob fetch con anello di caricamento, lerp normalizzato sul tempo, seek gated, scritture DOM solo al cambio, bande in vh validate col flick test, sistema di leggibilità a quattro strati, i cinque cancelli dell'eroe statico tenuti vivi coi change listener, pagina completa anche senza video, e tutto il quality floor di `scrub-pipeline.md`.

## 10. Il cancello della copy

Ogni riga qui sopra va nel sito parola per parola. Prima che qualcuno veda la pagina: zero trattini lunghi, zero parole da brochure, e nessun tic da AI nel corpo del testo.

# Bottega del Web

Sito dell'agenzia. Costruiamo siti per piccole attività locali: ristoranti, parrucchieri, dentisti, artigiani. Il cliente vede il sito finito **prima** di pagare. Se accetta: 179 € subito (primo mese più il dominio), poi 150 €/mese con tutto incluso.

La concorrenza sono le agenzie: 1.200 € di realizzazione più 150 €/mese, e le modifiche si pagano a parte.

## Regole tecniche

- Siti statici puri: HTML, CSS e JavaScript nel file, zero dipendenze, zero build step, zero npm install. Deve funzionare aprendo `index.html` con doppio clic.
- CSS dentro `<style>` nello stesso file. Font da Google Fonts.
- Mobile-first sempre: si progetta a 380px e si allarga.
- Tutti i testi in italiano.
- Deploy: push su `main`, Cloudflare Pages pubblica da solo (build command vuoto, output directory `/`).
- Le demo stanno in `demo/<categoria>/`.
- **Prima di ogni modifica al design, rileggere [DESIGN.md](DESIGN.md).**

# FAI Post Studio

Generátor příspěvků na Instagram Fakulty aplikované informatiky UTB.
Běží celý v prohlížeči: fotky ani texty se nikam neodesílají.

## Nasazení na GitHub Pages

1. Nahraj obsah této složky do repozitáře (do kořene, nebo do složky `docs/`).
   Soubor `.nojekyll` nahraj taky.
2. V repozitáři otevři **Settings → Pages**.
3. **Source:** Deploy from a branch. **Branch:** `main`, složka `/ (root)` nebo `/docs`.
4. Po minutě až dvou je aplikace na `https://<uživatel>.github.io/<repozitář>/`.

Aplikace nepotřebuje žádný build ani server, jde o statické soubory.

## Co je ve složce

| Soubor | K čemu |
|---|---|
| `index.html` | celá aplikace |
| `sample.jpg` | ukázková fotka při prvním spuštění |
| `fonts/` | písma uložená přímo na webu (žádné načítání z Google Fonts) |
| `mp/` | model pro „Najít osobu“ (MediaPipe; prohlížeč si stáhne asi 6 MB až při prvním použití) |
| `licenses/` | licence písem (SIL OFL 1.1) a modelu (Apache 2.0) |
| `favicon.svg` | ikonka v záložce prohlížeče |

## Dobré vědět

- **Rozpracované projekty a fotky** se ukládají v prohlížeči každého uživatele zvlášť.
  Kolegovi nebo ke schválení se posílá **soubor projektu** (Projekty → Uložit projekt do souboru).
- Úložiště prohlížeče patří k adrese webu. Všechny stránky na `<uživatel>.github.io`
  sdílejí jednu adresu, takže je lepší mít aplikaci jako jediný web na tomto účtu,
  nebo na vlastní doméně.
- Vyzkoušeno v Chromu na počítači i v mobilním zobrazení. Edge by se měl chovat stejně;
  Safari a Firefox nebyly testované, při potížích pomůže Chrome.

## Licence třetích stran

- Písma Geist, Geist Mono, Bricolage Grotesque, Unbounded, Syne, Archivo a JetBrains Mono:
  SIL Open Font License 1.1 (viz `licenses/font-*.txt`), soubory z projektu Fontsource.
- MediaPipe Selfie Segmentation: Apache License 2.0 (viz `licenses/mediapipe-Apache-2.0.txt`).

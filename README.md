Matchlight

Din highlight-video från Veo – gjord direkt i mobilen.

Matchlight är en webbapp för fotbollsspelare som vill göra en egen highlight-video av sina bästa situationer. Du väljer en matchvideo från Veo, klipper ut dina bästa ögonblick, markerar dig själv med en ring som följer dig i bilden och exporterar en färdig video som kan läggas upp på Instagram eller TikTok.

🔗 Live: https://matchlightfinland.github.io/Matchlight/

Utvecklas av Matchlight.

Så fungerar det
Matchvideo – Ladda ner matchen (eller ett enskilt klipp) som MP4 från Veo och välj filen i appen.
Dina klipp – Spela videon och tryck Start när något bra händer och Stopp när det är över. Bocka ur klipp du inte vill ha med.
Markera dig själv – Tryck på dig själv i början och slutet av varje klipp. Ringen följer dig däremellan. Lägg till fler punkter där du byter riktning.
Stil – Välj ringens färg och storlek, tempo (0,5×–1,5×), format (16:9 eller 9:16 som följer dig) och eventuell musik.
Exportera – Appen spelar upp klippen och spelar in dem till en färdig video som du sparar i telefonen.
Integritet

Ingen video laddas upp någonstans. All bearbetning sker lokalt i användarens webbläsare. Appen sparar bara små inställningar (språk och ringstil) i webbläsarens localStorage.

Teknik
En enda fil: index.html med HTML, CSS och JavaScript. Inget byggsteg och inga beroenden att installera.
Video renderas på en <canvas> och spelas in med MediaRecorder + captureStream().
Typsnitt: Barlow och Barlow Condensed från Google Fonts.
Språk: svenska, engelska, finska, norska, danska, tyska, spanska, franska, italienska, portugisiska och nederländska. Språket väljs automatiskt efter webbläsaren och kan bytas i appen.
Ljust och mörkt tema följer systemets inställning.
Webbläsarstöd
Webbläsare	Exportformat
Safari på iPhone	MP4 – redo att läggas upp
Chrome på dator/Android	WebM – fungerar på Instagram och TikTok, men iPhones Bilder-app kan behöva en konverterare
Köra lokalt

Klona repot och starta en enkel webbserver i mappen:

bash
git clone https://github.com/MatchlightFinland/Matchlight.git
cd Matchlight
python -m http.server 8000

Öppna sedan http://localhost:8000 i webbläsaren. Vill du testa på mobilen kan du öppna samma adress via datorns IP-adress när telefonen är på samma wifi.

Publicering

Appen publiceras med GitHub Pages från grenen main (rotmappen). Varje ändring som pushas till main går ut på live-adressen efter någon minut.

Tidig åtkomst

Appen har en enkel kodspärr för tidig åtkomst. Spärren ligger i klientkoden och är därför inget riktigt skydd – den är bara till för att hålla appen utanför allmän spridning under testperioden.

Kontakt

Frågor och feedback: robin@matchlight.fi

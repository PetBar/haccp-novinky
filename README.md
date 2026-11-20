# haccp-novinky

Zprávy z denního monitoringu HACCP pro web [haccpzpracovani.cz](https://haccpzpracovani.cz).

Soubor `novinky.json` každé ráno (Po–Pá) přepíše denní monitoring. Web si ho načítá
a zobrazuje v běžícím pásku a v sekci „Co se právě děje v gastru“.
Zprávy se vybírají a skrývají v zásobníku Monitoring HACCP, záložka **Na webu**.

Soubor needitujte ručně, další běh monitoringu by změny přepsal.

## Formát

```json
{
  "verze": 1,
  "aktualizovano": "2026-11-20T17:00:00+00:00",
  "zpravy": [
    {"id": "…", "datum": "RRRR-MM-DD", "zdroj": "…", "stitek": "Legislativa | Varování | Z praxe | …",
     "titulek": "na kartu, bez jmen malých provozoven", "kratky": "do pásku", "rada": "co to znamená pro provoz", "url": "…"}
  ],
  "terminy": [
    {"datum": "RRRR-MM-DD", "nazev": "…", "popis": "…"}
  ]
}
```

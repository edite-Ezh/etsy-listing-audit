# Etsy Listing Audit: Codex uzstādīšana un lietošana

## Kas vajadzīgs

- ChatGPT konts ar pieeju Codex/ChatGPT desktop lietotnei;
- Google Chrome;
- ChatGPT pārlūka paplašinājums;
- EverBee paplašinājums un aktīvs EverBee konts, ja vēlies redzēt tagu un pieprasījuma aplēses;
- Google Drive/Sheets pieslēgums tikai tad, ja gribi rakstīt atslēgvārdu tabulas tieši Google Sheets.

## 1. Instalē ChatGPT desktop lietotni

Lejupielādē lietotni no oficiālās OpenAI instrukcijas:

https://learn.chatgpt.com/docs/quickstart

Windows lietotāji var izmantot arī:

https://learn.chatgpt.com/docs/windows/windows-app

Atver lietotni un pieslēdzies savam ChatGPT kontam.

## 2. Pieslēdz Chrome

1. ChatGPT desktop lietotnē atver **Settings → Computer Use**.
2. Izvēlies Chrome un spied **Install**.
3. Chrome veikalā instalē ChatGPT paplašinājumu un pārskati tā prasītās atļaujas.
4. Atgriezies **Settings → Computer Use** un pārbaudi, vai pie Chrome redzams **Manage**.
5. Atļauj pieeju `etsy.com`. Neizvēlies pieeju visām vietnēm, ja tā nav vajadzīga tavai darba plūsmai.

Oficiālā instrukcija:

https://learn.chatgpt.com/docs/chrome-extension

## 3. Sagatavo EverBee

1. Instalē EverBee Chrome paplašinājumu.
2. Pieslēdzies savam EverBee kontam.
3. Atver Etsy sludinājumu un pārbaudi, vai redzi **Analyze listing**.
4. Atceries: EverBee Volume, Competition, Score, sales un conversion ir aplēses, nevis Etsy oficiālie dati.

Skill darbojas arī bez EverBee, bet tad analīzē nebūs pārbaudītu EverBee metriku.

## 4. Instalē Etsy Listing Audit skill

Codex sarunā ieraksti:

```text
$skill-installer Install the skill from https://github.com/edite-Ezh/etsy-listing-audit/tree/main/skills/etsy-listing-audit
```

GitHub repozitorijs: https://github.com/edite-Ezh/etsy-listing-audit

Pēc instalācijas atver jaunu sarunu. Ja skill neparādās, pārstartē lietotni.

## 5. Pārbaudi darbību

1. Chrome atver vienu Etsy sludinājumu.
2. Codex jaunā sarunā pievieno Chrome ar `@` izvēlni vai piemini atvērto cilni.
3. Ieraksti:

```text
Use $etsy-listing-audit to audit the Etsy listing in my open Chrome tab.
```

Vari rakstīt arī latviski:

```text
Izmanto $etsy-listing-audit un izanalizē Etsy sludinājumu manā atvērtajā Chrome cilnē.
```

Skill analizēs katru sludinājumu atsevišķi un beigās pajautās, vai sagatavot hero ideju atslēgvārdus EverBee pārbaudei.

## 6. Google Sheets pieslēgums — pēc izvēles

Google Sheets nav nepieciešams pašam auditam. Tas vajadzīgs tikai tad, ja gribi, lai rezultātu vai atslēgvārdus ieraksta tieši tavā tabulā.

1. ChatGPT/Codex pluginu vai savienojumu sadaļā pieslēdz Google Drive.
2. Autorizācijas logā izvēlies vajadzīgo Google kontu un pārskati pieprasītās atļaujas.
3. Izveido testa Google Sheet un iedod tā saiti Codex.
4. Vispirms palūdz nolasīt tabulas nosaukumu vai konkrētu diapazonu. Tikai pēc tam dod atļauju rakstīt datus.

Ja Google Drive nav pieslēgts, palūdz izveidot īstu `.tsv` failu. To var atvērt vai importēt Google Sheets, saglabājot divas kolonnas.

## 7. Droša lietošana

- Vienmēr pārskati pārlūka un Google konta atļaujas.
- Atļauj tikai tās vietnes un failus, kas vajadzīgi uzdevumam.
- Nepublicē klientu privātos datus vai paroles.
- Pirms mainīt Etsy sludinājumu, vispirms izmanto auditu un pārskati ieteikumus.

## Ja nevēlies instalēt Codex skill

Izmanto failu `FALLBACK-PROMPT-LV.txt` ChatGPT sarunā. Pievieno Etsy saiti un, ja nepieciešams, ekrānuzņēmumus ar EverBee tagiem, variantiem un piegādes datiem.


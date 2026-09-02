# Etsy Listing Audit

Atkārtoti izmantojams Codex skill Etsy sludinājumu auditam. Tas analizē vienu sludinājumu neatkarīgi pēc buyer intent, hero un galerijas signāliem, piedāvājuma skaidrības, EverBee datiem, cenas un piegādes.

## Ātra lietošana

1. Instalē skill no šī repozitorija ar Codex `$skill-installer`.
2. Pārstartē Codex vai atver jaunu sarunu, ja skill uzreiz neparādās.
3. Atver Etsy sludinājumu pārlūkā.
4. Raksti: `Use $etsy-listing-audit to audit the Etsy listing in my open browser tab.`

Tiešā instalēšanas frāze pēc repozitorija publicēšanas:

```text
$skill-installer Install the skill from https://github.com/edite-Ezh/etsy-listing-audit/tree/main/skills/etsy-listing-audit
```

GitHub repozitorijs: https://github.com/edite-Ezh/etsy-listing-audit

## Saturs

- `skills/etsy-listing-audit/` — standalone skill.
- `.codex-plugin/plugin.json` — plugin pakotnes manifests.
- `docs/CODEX-SETUP-LV.md` — dalībnieku uzstādīšanas instrukcija.
- `docs/FALLBACK-PROMPT-LV.txt` — garais prompts ChatGPT vai gadījumiem bez skill.
- `docs/WEBSITE-CONTENT-LV.md` — gatavs lapas saturs lejupielādēm.

## Piezīme par izplatīšanu

Standalone skill un ZIP ir piemērots meistarklasei un lokālai testēšanai. Plugin manifests ļauj to pašu metodoloģiju vēlāk iesniegt plašākai instalējamai izplatīšanai bez skill pārrakstīšanas.


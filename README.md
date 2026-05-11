# Tomos Releases

Deze repo bevat alleen **gebouwde IPA's** van [Tomos Dash](https://github.com/Woetner/tomos)
voor sideloading via [AltStore](https://altstore.io).

Source-code zit in de privé-repo `tomos`.

## AltStore source toevoegen

Open AltStore op je iPhone → **Settings** → **Sources** → **+** → plak:

```
https://raw.githubusercontent.com/Woetner/tomos-releases/main/altstore-source.json
```

AltStore checkt automatisch op updates. Nieuwe versies verschijnen als
"Update" knop bij Tomos Dash.

## Hoe het werkt

1. Code-wijzigingen worden gepusht naar de privé `tomos`-repo
2. GitHub Actions bouwt automatisch een nieuwe ongesigneerde IPA
3. De IPA wordt als release naar deze public repo gepubliceerd
4. `altstore-source.json` wordt bijgewerkt met de nieuwe versie + URL
5. AltStore-app op de iPhone ziet de update bij eerstvolgende refresh

## Privacy

IPA's zijn ongesigneerd — ze werken alleen na re-signing met je eigen
Apple ID via AltStore. Iemand anders die de IPA downloadt kan hem niet
zomaar op zijn iPhone draaien zonder zijn eigen Apple ID.

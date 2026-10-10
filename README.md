# Munch – Pac-Man játék különleges szellemekkel

Böngészőben futó Pac-Man-szerű játék, egyetlen `index.html` fájlban (külső függőség nélkül).
A feladat csavarja: **minden szellemnek van egy egyedi képessége**, ami megváltoztatja a játékmenetet.

## A szellemek képességei

| Szellem | Képesség | Mit változtat a játékon? |
|---|---|---|
| **Blink** (piros) | Teleportálás | ~10 másodpercenként kijelöl egy pontot a közeledben (villogó piros kör), majd 1 másodperc múlva odaugrik. Nem lehet sarokba szorítani, és nem lehet rá kiszámíthatóan várni. |
| **Phase** (rózsaszín) | Falakon átjárás | 3 másodpercre áttetszővé válik és átmegy a falakon, utána vissza kell találnia a folyosóra. A labirintus "zárt" részei sem biztonságosak. |
| **Goo** (cián) | Ragacsnyom | Minden mező, amin végigmegy, ragacsos lesz, és ~6 másodpercig lassítja Pac-Mant. A pálya fokozatosan "beszennyeződik", az útvonaltervezés számít. |
| **Gardener** (narancs) | Pontok újratelepítése | Visszaülteti a már megevett pontokat, így a pálya nem ürül ki magától. Muszáj elkapni/elkerülni, különben végtelenül nyúlik a szint. |

Amíg a szellemek kék (megijedt) állapotban vannak, a képességeik szünetelnek.

## Irányítás

- Nyilak vagy WASD: irányítás (telefonon: húzás a pályán vagy a képernyő D-padje)
- `P` / `Esc`: szünet, `M`: hang ki/be, `Enter` / koppintás: indítás

## Egyéb funkciók

Négy különböző AI-személyiség (üldöz, előre céloz, bekerít, bizonytalankodik), power pellet és szellemevés
kombóval, bónusz gyümölcs, extra élet 10 000 pontnál, alagút, szintenként gyorsuló játék, mentett high score,
hangeffektek (WebAudio).

## Futtatás

Nyisd meg az `index.html` fájlt egy böngészőben. GitHub Pages-en is fut (lásd lent).

---

## English summary

A browser-based Pac-Man-style game in a single `index.html`. Every ghost has a unique ability:
**Blink** teleports next to you after a one-second warning, **Phase** walks through walls for 3 seconds,
**Goo** leaves a sticky trail that slows Pac-Man, and **Gardener** replants the dots you have already eaten.

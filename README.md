# Markdown Viewer

Jednoduchý a rýchly prehliadač Markdown súborov pre Windows – iba na čítanie. Jeden EXE súbor, nič sa neinštaluje.

Pre Windows 10 (2004+) a Windows 11, x64.

## Stiahnuť

[Stiahnuť MarkdownViewer.exe](https://github.com/enthilza/MarkdownViewer/releases/latest/download/MarkdownViewer.exe) · [Všetky vydania](https://github.com/enthilza/MarkdownViewer/releases)

Samostatné EXE obsahuje .NET runtime, nič sa neinštaluje. Ulož ho do priečinka, kde máš právo zapisovať, a spusti. Súbor otvoríš cez `Ctrl+O`, pretiahnutím do okna alebo cez „Otvoriť v programe“.

## Čo vie

- nadpisy, odseky, citácie, vnorené zoznamy a zoznamy úloh, tabuľky so zarovnaním, bloky kódu,
- odkazy na nadpisy v dokumente a na ďalšie Markdown súbory, lokálne obrázky,
- svetlá a tmavá schéma, voľba typu a veľkosti písma (`Ctrl++`, `Ctrl+-`, `Ctrl+0`, `Ctrl+koliesko`),
- hľadanie v dokumente (`Ctrl+F`, ďalší výskyt `Enter` alebo `F3`) bez ohľadu na veľkosť písmen a diakritiku,
- voliteľné priehľadné okno so zaoblením a tieňom (ponuka Nastavenia; predvolene vypnuté, obyčajné okno je rýchlejšie),
- zmenený súbor sa obnoví sám, ručne klávesom `F5`,
- text sa dá označiť a kopírovať,
- okno si pamätá polohu, veľkosť a monitor.

## Bezpečnosť

Nič z dokumentu sa nespúšťa – surové HTML ani skripty sa nevykonávajú, zobrazia sa ako text. Obrázky z internetu sa nenačítavajú, takže samotné otvorenie dokumentu nevyvolá žiadnu sieťovú komunikáciu. Odkazy `http`, `https` a `mailto` sa otvoria v predvolenej aplikácii až po kliknutí; ostatné schémy a sieťové cesty sú blokované.

## Aktualizácie

Aplikácia pri štarte overí, či existuje novšie vydanie, a tlačidlom aktualizácie to môžeš skontrolovať aj ručne. Inštaluje sa až po tvojom potvrdení.

Každé vydanie obsahuje `MarkdownViewer.exe`, `update.json` a `update.sig`. Aplikácia overí digitálny podpis popisu vydania (RSA/SHA-256) zabudovaným verejným kľúčom a potom veľkosť, kontrolný súčet SHA-256 a verziu stiahnutého EXE. Nové EXE musí pred výmenou úspešne naštartovať na skúšku; ak nenaštartuje, pôvodná verzia ostane nedotknutá.

Nejde o Windows Authenticode podpis, preto môže Windows SmartScreen pri prvom spustení zobraziť upozornenie.

## Súkromie

Kontrola aktualizácií kontaktuje iba GitHub. Nastavenia sú v `%LOCALAPPDATA%\MarkdownViewer`.

Tento repozitár obsahuje iba distribučné súbory a informácie o vydaniach.

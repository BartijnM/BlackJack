# BlackJack

Ik bouw een lokaal blackjackspel waarin ik tegen een dealer speel met fictieve punten. Met een optionele teller kan ik oefenen met Hi-Lo op de kaarten die ik tijdens het spel zie. Ik speel in een eigen desktopvenster met visuele speelkaarten, een kaartachterkant voor de dichte dealerkaart en actieknoppen.

## Lokaal starten

Ik gebruik Python 3.11 of nieuwer. In PowerShell voer ik vanuit de hoofdmap uit:

```powershell
py -m venv .venv
.\.venv\Scripts\python.exe -m pip install -e .
.\.venv\Scripts\python.exe -c "import blackjack_game"
```

Ik controleer Tkinter met `.\.venv\Scripts\python.exe -m tkinter`. Dit opent een testvenster. Het spelvenster volgt in de eerste bouwstap. De eerste spelstap staat in de roadmap.

- [Architectuur](docs/architectuur.md)
- [Roadmap](docs/roadmap.md)
- [Voortgang](docs/voortgang.md)

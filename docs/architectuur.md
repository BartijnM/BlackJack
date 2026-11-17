# Architectuur

Ik geef kaarten, handen en de schoen een eigen model. De schoen deelt kaarten uit en schudt tussen rondes als dat nodig is. De hand bepaalt het totaal, met een aas als 1 of 11. De ronde beslist welke acties beschikbaar zijn en bepaalt de uitkomst. De Tkinter-interface tekent kaartvlakken met rang en kleursymbool voor speler en dealer. Voor de dichte dealerkaart tekent hij een kaartachterkant. Knoppen voor Kaart, Passen en Nieuwe ronde geven acties door aan de ronde en worden ingeschakeld als die acties beschikbaar zijn. Een schakelaar bepaalt of de telling zichtbaar is.

De teller verwerkt iedere zichtbare kaart precies één keer, inclusief de dichte dealerkaart zodra die wordt omgedraaid. Ik zet de telling bij het schudden op nul. De running count is de som van +1 voor 2–6, 0 voor 7–9 en −1 voor 10, plaatjes en aas. Voor de true count deel ik door het geschatte aantal resterende decks, met expliciet gedrag bij een lege schoen.

Ik begin met hit en stand, een dealer die past op elke 17, en een natuurlijke blackjack als aparte uitkomst. Daarna voeg ik inzet met fictieve punten, dubbelen en splitsen toe. Met vaste kaartvolgordes kan ik ronde-uitkomsten en de teller reproduceren.

Ik voeg modules aan `src/blackjack_game/` toe zodra ik ze nodig heb. Met `unittest` controleer ik de spelregels en beslissingen zonder een venster te openen.

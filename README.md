﻿🎓 Workshop: Skapa en knapp som tänder en lampa i Unreal Engine

Tid: 30 minuter
Mål: Lära sig att använda Blueprints för att interagera med objekt (t.ex. tända/släcka ljus med en knapp)

🛠️ Steg-för-steg
1. Skapa projektet (5 min)

    Starta Unreal Engine

    Välj Games → First Person Template

    Döp projektet (t.ex. "LampKnappWorkshop")

    Klicka på "Create"

2. Lägg till en lampa i världen (5 min)

    I Place Actors-panelen, dra in en Point Light i scenen

    Placera den där du vill att lampan ska lysa

    Döp ljuset till MyLamp i World Outliner

    I detaljer-panelen: Inaktivera "Visible" så att den startar släckt

3. Skapa en knapp (10 min)

    Högerklicka i Content Browser → Blueprint Class → Actor → döp den till BP_Button

    Öppna BP_Button:

        Lägg till en Static Mesh (ex: kub) → detta är själva knappen

        Lägg till en Box Collision ovanpå knappen

📘 Lägg till funktionalitet:

    Välj Box Collision → i detaljerpanelen scrolla till Events

        Klicka på OnComponentBeginOverlap

    I eventgraph:

        Lägg till en "Get All Actors of Class" (sök efter Point Light)

        Dra ut och sätt "Set Visibility" på ljuset

        Använd en FlipFlop-nod för att kunna växla mellan av/på

4. Placera knappen i världen (5 min)

    Dra in BP_Button i världen

    Placera den nära där spelaren kan nå den

    Kör spelet (Play) och testa!

🎯 Extra utmaningar (om tid finns)

    Lägg till ett ljud när knappen trycks

    Använd en Timeline för att animera knappen inåt vid tryck

    Byt färg på ljuset när det är tänt

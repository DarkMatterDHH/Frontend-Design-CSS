# Refleksion over `:has()`

Jeg synes `:has()` er en god løsning i denne opgave, fordi den gør det muligt at style kortet ud fra dets indhold i stedet for at tilføje ekstra CSS-klasser i HTML’en. Det holder markupen renere og mere semantisk, fordi hvert kort behøver ikke at kende til, hvilken variant det er. I stedet kan browseren selv læse strukturen og anvende den rigtige stil.

Det gør også koden lettere at vedligeholde. Når indholdet ændrer sig, behøver vi ikke at huske at opdatere mange klasser i HTML’et eller holde styr på flere varianter i CSS. Reglerne bliver mere naturlige, fordi de beskriver relationen mellem parent og child, fx “kort uden billede” eller “kort med overskrift”. Det gør koden mere læsbar for andre udviklere, da den afspejler den faktiske struktur i komponenten.

I denne opgave er `:has()` især nyttigt, fordi kortene ser forskelligt ud afhængigt af om de har et billede eller en overskrift. Hvis vi havde brugt ekstra klasser i HTML’en, ville det være mere omstændigt og lettere at fejlkonfigurere. Med `:has()` bliver CSS mere deklarativt og lettere at forstå, samtidig med at HTML’en forbliver enkel og ren.

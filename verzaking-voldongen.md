```mermaid
---
title: Voldongen verzaking
---
graph TD
    A{Heeft de overtredende partij de slag van de verzaking of een volgende slag gemaakt?}
    A -->|Nee| B[Geen rechtzetting]
    A -->|Ja| C{"Was de verzaking een tweede verzaking in dezelde kleur (die voorgespeeld is)?"}
    C -->|Ja| D[Negeer de tweede verzaking. Enkel de eerste verzaking wordt behandeld.]
    C -->|Nee| E{Was de verzaking in dummy of een andere kaart die gespeeld moest worden en die met de beeldzijde naar boven lag voor de slag begon?}
    E -->|Ja| F[Geen rechtzetting tenzij tegenpartij recht had op meer slagen zonder verzaking] -->P["Contacteer de wedstrijdleider met alle gespeelde slagen. (Laat de kaarten zitten zoals ze gespeeld zijn en noteer alle slagen achteraf.)"]
    E -->|No| G{Werd de verzaking opgemernt na een bieding door niet-overtredende partij in het volgende spel of nadat de ronde is geëindigd?}
    G -->|Ja| F
    G -->|Nee| H{Hebben beide paren verzaakt?}
    H -->|Ja| P
    H -->|Nee| J[De tegenstrevers krijgen 1 slag van de overtreders.]
    J --> K{Heeft de overtredende partij slechts 1 slag gemaakt na de verzaking?}
    K -->|Ja| L[Geen verdere rechtzetting]
    K -->|Nee| M{Heeft de overtredende SPELER de slag van de verzaking gewonnen (door te troeven)?}
    M -->|Ja| N[De tegenstrevers krijgen een tweede slag van de overtreders.]
    M -->|Nee| O[Denkt de niet-overtredende partij meer slagen te kunnen maken zonder de verzaking dan degenen waarmee ze gecompenseerd werden?] -->P
    N --> O
    L --> O
```

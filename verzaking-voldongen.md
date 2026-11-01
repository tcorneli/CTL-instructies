```mermaid
---
title: Voldongen verzaking
---
%%{init: {"flowchart": {"defaultRenderer": "elk", "wrappingWidth": 450, "nodeSpacing": 30, "rankSpacing": 40}}}%%
graph TD
    classDef default fontSize:18px,padding:15px,line-height:1.4;

    A{{Heeft de overtredende partij de slag van de verzaking<br>of een volgende slag gemaakt?}}
    A -->|Nee| B[Geen rechtzetting]
    A -->|Ja| C{{"Was de verzaking een tweede verzaking in dezelde kleur<br>(die voorgespeeld is)?"}}
    
    C -->|Ja| D[Negeer de tweede verzaking.<br>Enkel de eerste verzaking wordt behandeld.]
    C -->|Nee| E{{Was de verzaking in dummy of een andere kaart die<br>gespeeld moest worden en die met de beeldzijde<br>naar boven lag voor de slag begon?}}
    
    E -->|Ja| F[Geen rechtzetting tenzij tegenpartij recht had<br>op meer slagen zonder verzaking]
    F --> P["Contacteer de wedstrijdleider met alle gespeelde slagen.<br>(Laat de kaarten zitten zoals ze gespeeld zijn en noteer alle slagen achteraf.)"]
    
    E -->|Nee| G{{Werd de verzaking opgemernt na een bieding door<br>niet-overtredende partij in het volgende spel of<br>nadat de ronde is geëindigd?}}
    
    G -->|Ja| F
    G -->|Nee| H{{Hebben beide paren verzaakt?}}
    
    H -->|Ja| P
    H -->|Nee| J[De tegenstrevers krijgen 1 slag van de overtreders.]
    
    J --> K{{Heeft de overtredende partij slechts 1 slag<br>gemaakt na de verzaking?}}
    
    K -->|Ja| L[Geen verdere rechtzetting]
    K -->|Nee| M{{"Heeft de overtredende SPELER de slag<br>van de verzaking gewonnen (door te troeven)?"}}
    
    M -->|Ja| N[De tegenstrevers krijgen een tweede slag<br>van de overtreders.]
    M -->|Nee| O[Denkt de niet-overtredende partij meer slagen<br>te kunnen maken zonder de verzaking dan degenen<br>waarmee ze gecompenseerd werden?]
    
    O --> P
    N --> O
    L --> O

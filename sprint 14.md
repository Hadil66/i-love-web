# Sprint 14 Lose Your Head
  ## Week 5
  ## Maandag 23 september
  Het gebruik van JAMstack, met JavaScript en API's, maakt het mogelijk om een modulaire architectuur te implementeren. Het voordeel hiervan is dat verschillende delen van een website of webapplicatie kunnen worden gebouwd en onderhouden door verschillende teams. Dit maakt het veel eenvoudiger om websites en webapplicaties te ontwikkelen en te onderhouden.
        
Enkele populaire headless CMS'en zijn: Directus, Prismic en WordPress.
        
   Site generators die je kunt gebruiken zijn: mdBook en Eleventy.
             **Verlies je hoofd.**
        
  ### Fabrique; Qatar Museums Project
  **Voorkeursstack:**      
        - SvelteKit
        - Directus
        **Leervragen:**
        - Hoe gebruik ik externe bibliotheken?
        - Hoe kan ik complexere JavaScript gebruiken?
        ### Briefing Voorbereiden
        
**Vragen voor Marko:**
        - Wat is de aanleiding van deze opdracht?
        - Wat voor API moeten we gebruiken?
        - Maakt het uit in welk framework we werken?
        - Hebben jullie een huisstijl waar we ons aan moeten houden?
        - Wat is het hoofddoel van de website?
        - Zijn er specifieke functies die jullie op de site willen hebben?
        - Hoe willen jullie dat de gebruiker de website ervaart?
        - Wie zijn de eindgebruikers van de website?
        - Is het een must om alle features op de website te hebben?
        - In hoeverre mogen wij afwijken van het ontwerp?
                ## Dinsdag 24 september
        
  ### Briefing @ Fabrique      [Bekijk de briefing](https://github.com/user-attachments/assets/b851f419-1dea-4480-9001-d09ab40d8fcd)
        
  ### Debrief   
  ![Debrief afbeelding](https://prod-files-secure.s3.us-west-2.amazonaws.com/4d2d2910-0f35-4885-8674-f6228a3ebfa0/a7417f2f-edf3-4a9a-a915-d8c714cb672f/370692682-5e2dc532-0c35-407c-91ef-6d6fae1bb2d2.png)
            ## Woensdag 25 september
          **Intersection Observer.**
        Centraal een div plaatsen:
```
     <body>
            <div></div>
     </body>
 ```
        
   **Filteren met de Directus API:**
              ```
/items/person/?filter={"squad_id": 3}
        ```
        
  ## Donderdag 26 september
  ### Infinite Scroll / Canvas Research
  Er is een [infinite scroll plugin](https://infinite-scroll.com/), een JavaScript-plugin die automatisch de volgende pagina toevoegt, zodat gebruikers niet een volledige pagina hoeven te laden. Dit laadt nieuwe content wanneer je aan het einde van de pagina komt.
        - Gebruik geen `<canvas>`, dat zegt niet veel.
        - Geen muiswiel om te zoomen.
        - Gebruik transformaties zoals **translate** en **scale**.
        - Gebruik **viewportTransform** om panning en zoom bij te houden.
        - **Panning:** Het verplaatsen van de inhoud van de canvas door het bijhouden van muisbewegingen en het updaten van de coördinaten van de canvas.
        - **Zooming:** In- en uitzoomen met behulp van het muiswiel, waarbij de scale-factor wordt aangepast om de weergave te vergroten of te verkleinen.
        - **fabric.js**
        - **konva.js**
        
   [Masonry Infinite Grid](https://naver.github.io/egjs-infinitegrid/Guides)
              [Infinite Canvas Gids](https://infinite-canvas.org/guide.html)
        
  [Canvas Panning en Zooming](https://harrisonmilbradt.com/articles/canvas-panning-and-zooming)
              - Afbeeldingen inladen en daarna herhalen?
        - **Vraag:** Hoe willen we zoomen? Met behulp van knoppen?
        
  ## Vrijdag 27 september
  ### Voortgangsgesprekken met CMD-studenten
  **Feedback ontvangen van:**
        - **Dirk:** Goed gebruik van custom properties. Read.me niet af; alt-tekst ontbreekt.
        - **Lotte:** JavaScript-like button; vragen over dark en light mode.
        - **Emma:** Eerste pagina niet af; geen JavaScript (menu); geen custom properties.
        - **Jannie:** Styling aanpassingen nodig; CSS evalueren.
        - **Caia:** Goed gebruik van custom properties; dark-mode kleuren moeten in CSS.
        - **Joy:** Lettertype niet herkend; geen custom properties; Read.me ontbreekt.
        - **Jilke:** Kleine JavaScript-fout; goed gebruik van custom properties.
        
  **Feedback van Krijn en Charley:**
        
  - Klein beginnen: eerst de view en dan infinite.
  - **Wat is de core functionaliteit?**
  - User story: Als gebruiker wil ik 30 afbeeldingen zien.
  - Enhancement = infinite.
  - Moscow toepassen.
  - Poker! voor infinite scroll.
  - Pull requests afspraken.
  - Mergen.
  - Let op dingen die geen eind hebben (niet infinite researchen).
  - Maak navigatie.
  - Practical scroll snapping.
        
      **Weekend Planning:**
      
      - Zaterdag: HTML
      - Zondag: CSS/JS
      


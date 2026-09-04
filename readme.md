i min kod använder jag grid 
.tabla{
    display: grid;
    grid-template-columns: 1fr 1fr 1fr ;
    gap: .5rem;
}
jag använder grid för att jag behöver ordna information av avgångtavaln i rader och kolumner.

jag använder flexbox i koden 
.kort-rad {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
}
flexbox ska ordna korten i en riktning. distination korten ska ligga brevid varandra. flex wrap för korten ska flytta till ny rad när det finns inte plats. gap gör att göra mellanrum mellan korten.

om jag använder flex på .tabla det blir en rad och införmation kommer att kläms.

 för .kort-rad det går att använda grid men det är onödigt för att distinationkorten behöver bara en rad.

 Ägarskap

Jag kan förklara varje rad jag har pushat och AI är ett verktyg – inte en ersättning för förståelse

 1. Varför sitter display: grid på .tabla och inte på varje .avgang?
  grid ska sitta på föräldern element .tabla  för att grid organisera all child elemnt .avgang i rader och kolumner

2. Vad gör 1fr jämfört med width: 33% på varje cell?
1 fr delar mellan grid kolumner 1fr 1fr 1fr får tre kolumner lika mycket plats.

3. Vad händer om href="#tabla" pekar rätt men section saknar id="tabla"?
det ska inte hoppa någonstans.

4. Varför behöver tabla en media query men destinationer ofta klarar sig med flex-wrap?
.tabla har tre kolumner, så på en liten skärm  det ändras till en kolumn med en media query.

Destinationerna använder flex-wrap, så korten kan flytta ner när skärmen blir mindre.

Jag testade på 375px. Tabla visade en kolumn och media query var aktiv
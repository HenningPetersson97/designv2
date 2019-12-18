Laddningstider
=======================

Detta kursmomentet handlar om laddningstider på en webbplats samt om hur användbar webbplatsen är. Jag ska jämföra tre olika webbplatser och se vilket resultat jag kan få fram.

Urval
-----------------------

Jag valde att undersöka expressen, aftonbladet och smålandsposten eftersom de är alla tidningar. Jag ville jobba med tre hemsidor som hade samma syfte för att se ifall jag kunde hitta några likheter eller vad de har gjort annorlunda från varandra när det gäller laddningstider och användbarhet.

Metod
-----------------------

Jag använde mig av google chrome när jag undersökte mina hemsidor. Jag använde mig av devtools för att kunna se hemsidornas network som visar hur många requests det finns på hemsidan samt mängden resources och sidans loadtimes. Jag använde mig också av pagespeed insights som är baserad på "lighthouse" som redan finns inbyggd i google chromes devtools men jag tycker att det är lättare att analyzera hemsidorna med hjälp av pagespeed insights.

All data har jag samlat i ett google excelark som du hittar [här](https://docs.google.com/spreadsheets/d/1d9I9GW49xv45c2QkSOF2hDd5WfGsnjhTvTkDmQEu7Hk/edit?usp=sharing).

Resultat
-----------------------

[FIGURE src="image/aftonbladet.png?w=500" caption="Aftonbladet"]

De tre sidorna som jag har undersökt:
[Startsida](https://www.aftonbladet.se/)
[Sportbladet](https://www.aftonbladet.se/sportbladet)
[Nöjesbladet](https://www.aftonbladet.se/nojesbladet)

Det som aftonbladet har som störst problem med är storleken på vissa av deras sidor så som Nöjesbladet och startsidan. De borde också förbättra tiden det tar för dem att tolka, kompilera och köra JS-kod eftersom det är mycket JS-resurser som skickas. De borde också använda sig av mindre DOM-träd. De borde också ta bort resurser som blockerar renderingen på hemsidan.

[FIGURE src="image/expressen.png?w=500" caption="Expressen"]

De tre sidorna som jag har undersökt:
[Startsida](https://www.expressen.se/)
[Sport](https://www.expressen.se/sport/)
[Nöje](https://www.expressen.se/noje/)

Expressen ser bra ut men en förbättring hade varit att undvika ett stort DOM-träd. De skulle också kunna använda sig av modernarna bildformat.

[FIGURE src="image/smalandsposten.png?w=500" caption="Smålandsposten"]

De tre sidorna som jag har undersökt:
[Startsida](http://www.smp.se/)
[Sport](http://www.smp.se/sport/)
[Växjö](http://www.smp.se/vaxjo/)

Smålandsposten har ganska många förbättringar de skulle kunna göra. De borde ladda bilder på ett modernare sätt och dessutom använda lat inläsning på de bilder som ligger utanför skärmen. De borde också använda rätt storlek på sina bilder.

Analys
-----------------------

Det var intressanta resultat eftersom jag fick ganska olika resultat på de olika sidorna. Aftonbladet och smålandsposten va de sidor som hade mest problem och det var till största delen bilder som inte hade rätt format eller laddas in på ett dåligt sätt. Expressen klarade sig bra och det mesta såg bra ut på webbplatsen men sen om man jämför storleken på expressen och de andra hemsidorna så ser man att expressen har en mycket mindre storlek på sin hemsida än vad aftonbladet och smålandsposten har. Det gör så att expressen har lättare för att klara sig undan eftersom det inte finns lika mycket på webbplatsen som de andra har.

Alla tre webbplatser hade ett mycket bättre resultat på datorn än va de hade på mobilen. Expressen hade ändå ett acceptabelt resultat för mobiler men både aftonbladet och smålandsposten var katastrof. Även om aftonbladet klarade sig undan lite bättre än smålandsposten så har de ungefär samma problem. Smålandsposten använder sig inte av moderna bildformat och det gör att hemsidan jobbar mycket långsammare. Aftonbladet har resurser som blockar sin rendering och de har bilder som laddas som inte syns på sidan som gör att den jobbar långsammare.

Alla tre hemsidor skulle kunna förbättra sina laddningstider om de ändrade sina bildformat och hur de laddas på hemsidan. Även att expressen klarar sig bra genom testet så har den samma förbättrings förslag som de andra sidorna har. Det tyder på att expressen klarar sig undan eftersom storleken på hemsidan är mycket mindre än de andra två hemsidorna och använder sig av färre bilder.

Om jag skulle rangordna mina val av hemsidor så är det helt klart expressen som vinner men jag kan ändå hitta samma likheter i förbättringar för de hemsidor som fick ett sämre betyg i mätningen.

Egen uppfattning om laddningstid
-----------------------

Om en hemsida har en laddningstid mellan 2-3 sekunder så är det godkänt ifrån mig. Det var ingen hemsida som klarade av det helt men expressen kom väldigt nära. Aftonbladet hade laddningstider på över 10 sekunder som är alldeles för lång tid för att en hemsida ska ladda. Smålandsposten låg runt 4 sekunder och tycker att det kan vara ok. När jag refreshar sidorna så tycker jag ändå att jag knappt märker någon skillnad på dem och att de verkar vara snabbare än va de egentligen är, speciellt aftonbladet.

Övrigt
-----------------------

Rapporten är gjord av mig Henning Petersson.

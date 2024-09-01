# Övningar för vecka 2.

### git 
I veckans övningsmapp har jag lagt till en fil .gitignore. Denna säger vilka filer och eller mappar som ej ska syncas in i git.  
Så här har jag lagt till `.env` & `venv` då man inte bör ha med hela ens python miljö i syncen, utan istället ha en requirement fil till vilka bibliotek som behövs för att köra för att minska mängden filen som syncas.  
[Gitignore Docs](https://git-scm.com/docs/gitignore)

Det går även att sätta upp en global git ignore fil så behöver man inte lägga till denna information i alla ens projekt. [Guide](https://stackoverflow.com/questions/7335420/global-git-ignore)

### Power bi. 

#### Rest Övning ifrån vecka 1. 
Power bi övningen med hur anställda har flyttat mellan avdelningar ifrån vecka 1 ser vi till att göra under vecka 2.  
[Power bi v01](https://github.com/sebCoreChange/v01?tab=readme-ov-file#edits)  
Och gör då följande delar:  
Vem har jobbat flest av delningar?

- Vilken avdelning var störst 2024 Feb?
- Ta fram en rapport för desktop där man kan följa för en given avdelning och månad:
  - Antal individer
  - Antal nya
  - Antal avslutade
- i angiven period, förgående år och differensen där i mellan.

#### Övning 1.
Läs på om sankey diagram, som är en typ av flödesdiagram. [Docs MS Sankey](https://github.com/Microsoft/powerbi-visuals-sankey)  
De kräver att datan masseras en hel del för att fungera så försök sätta ihop det datasetet som krävs, och visualisera vart väljarna gick mellan 2 val. 
Bifogar en lite avstädad valu data set i data/valu_cleaned.csv 

#### Övning 2. 
Testa med ett eget dataset att sätta upp en sankey i power bi. Ni kan välja ett eget dataset eller ge er på hela valu datasetet.  
Om ni vill ha en bra prep övning på intressant data rekommenderar jag att preppa datan själv o kanske då visa fler än bara 2 år.  
[Valu 2022 Dataset](https://snd.se/sv/catalogue/dataset/2023-101-1) 

Om ni väljer att inte titta vidare på valu datan så välj ett annat dataset som man kan visa som flöden. 
- Näringsvärden till en sockerkaka över ingredienser? 
- Resultaträkning?
- utgå ifrån förra veckans övning o visa hur anställda rör sig mellan avdelningar. 
- eller något annat dataset ni känner för. 

### Python 

#### Övning 3. 
Säkerställ att ni i övnings mappen har en python envorment o att den är aktiv. 

#### Övning 4. 
Ni har fått sales data för de första 3 månaderna, men då ni glömde ange vid beställning vilken fil typ så har ni nu fått en rad olika filer.  
Börja med att sätta upp en jupyter notebook för o använd den för att kunna läsa in alla olika fil typer in till dataframes för att sätta samman dem till en enda, och skriv sedan ut filen till data_out/sales2024.csv. 

se till att ha följande funktion 
- read_csv  
- read_json  
- read_xlsx  

De ska ta ett filnamn in och returnera en dataframe. 
För att skriva så vill vi skapa följande funktioner:  
- write_csv
- write_xlsx

Som ska ta emot en dataframe samt ett filnamn och skriva det till formatet.  

Vad är den totala försäljningen under året?
Ta fram ett diagram med runnings sales i ett diagram. 

Ta fram ett diagram som även visar sales för varje månad. 

Vilken produkt har sålt bäst under året? (Anta att sales är försäljnings antal. )
Visa i ett bardiagram. 

Vilken produkt har haft största förändringen mellan första o sista månaden i försäljning? 
Går det att visa i någon form av visualisering?


##Harjoitus 5

###1. Käsitteet

1. Näkymä:
Ohjelmanäkymä jossa voi olla mm. työstämisalue, valikoita ja työkalupalkkeja. Näkymä on graafinen ja osa käyttöliittymää.

2. Wireframe:
On yksinkertainen graafinen esitys tai rautalankamalli ohjelman tai nettisivun toiminnallisuudesta ja ominaisuuksista.

3. Mockup:
Tarkempi graafinen luonnos ohjelman ulkoasusta kuin wireframe. Voi sisältää esimerkiksi käyttöliittymäelementtejä, valikkoja, työkalupalkkeja ja työstämisalueita.

4. Prototyyppi:
On ainakin osittain toimiva ohjelmaversio josta löytyy perustoiminnallisuus. Prototyypissä kaikki ominaisuudet eivät yleensä ole viimeisteltyjä ja esiintyy bugeja.

###2. Näkymät
1. Miten käyttötapaukset ja käyttöliittymät voisi yhdistää toisiinsa vaatimusmäärittelydokumentaatiossa?
Käyttötapaukset ja käyttöliittymänäkymät voidaan yhdistää toisiinsa wireframe mallissa.

2. Listaa järjestelmän käyttöliittymän olennaisimmat näkymät.
Aloitusnäkymä
- pelinäkymä
- asetukset
- pisteet

3. Kuvaile näkymät sanallisesti: mitä näkymällä tehdään ja mitä siinä näkyy. Pyri määrittelemään tässä 
näkymät toiminnallisesta näkökulmasta, älä niinkään ajattele miltä ne näyttävät
- Aloitusnäkymässä on pelin logo, taustakuva ja kolme nappia joista päästään aloittamaan peli, säätämään asetuksia ja katsomaan pisteitä.
- Pelinäkymässä on 2D karttanäkymä jossa näkyvät muut pelaajat ja vallattavat alueet erivärisinä, alueiden valtauksen aikalaskuri sekä löydetyt "extrat". Lisäksi tiimikohtaiset pisteet.
- Asetusnäkymästä löytyvät peliasetukset, kuten pelaajien määrä, laitteiden yhdistäminen peliin, valtausalueiden määrittäminen sekä erän kesto ja pelimoodi.
- Pistenäkymässä näkyvät pelaajien pisteet sekä omat parhaat pisteet kautta aikojen.

4. Määritä näkymien väliset siirtymät korkealla tasolla, mistä näkymästä pääsee minnekin? Millä tavoin visualisoisit tilasiirtymät?
Aloitusnäkymä
-> aloita peli -> peliasetukset -> pelinäkymä
-> omat asetukset
-> pisteet

Pelinäkymä
->aloitusnäkymä
->omat asetukset

Omat asetukset -> pelinäkymään jos peli on käynnissä tai aloitusnäkymään

Pisteet -> aloitusnäkymä

Tilasiirtymien välissä olisi 3Dzoom-fadein. Pelin käynnistämisen jälkeen aloitusruutu ennen kuin peli lataa. Pelin loputtua loppuruutu jossa näkyy voittanut tiimi ja kaikkien tiimien pisteet. Pelinäkymien välissä fade-to-black.

5. Listaa jokaista näkymää kohti tieto siitä, millaista tietosisältöä tai data käyttöliittymässä näytetään.




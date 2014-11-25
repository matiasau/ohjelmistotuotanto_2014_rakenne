

##Harjoitus 5

###1. K�sitteet

1. N�kym�:
Ohjelman�kym� jossa voi olla mm. ty�st�misalue, valikoita ja ty�kalupalkkeja. N�kym� on graafinen ja osa k�ytt�liittym��.

2. Wireframe:
On yksinkertainen graafinen esitys tai rautalankamalli ohjelman tai nettisivun toiminnallisuudesta ja ominaisuuksista.

3. Mockup:
Tarkempi graafinen luonnos ohjelman ulkoasusta kuin wireframe. Voi sis�lt�� esimerkiksi k�ytt�liittym�elementtej�, valikkoja, ty�kalupalkkeja ja ty�st�misalueita.

4. Prototyyppi:
On ainakin osittain toimiva ohjelmaversio josta l�ytyy perustoiminnallisuus. Prototyypiss� kaikki ominaisuudet eiv�t yleens� ole viimeisteltyj� ja esiintyy bugeja.

###2. N�kym�t
1. Miten k�ytt�tapaukset ja k�ytt�liittym�t voisi yhdist�� toisiinsa vaatimusm��rittelydokumentaatiossa?
K�ytt�tapaukset ja k�ytt�liittym�n�kym�t voidaan yhdist�� toisiinsa wireframe mallissa.

2. Listaa j�rjestelm�n k�ytt�liittym�n olennaisimmat n�kym�t.
Aloitusn�kym�
- pelin�kym�
- asetukset
- pisteet

3. Kuvaile n�kym�t sanallisesti: mit� n�kym�ll� tehd��n ja mit� siin� n�kyy. Pyri m��rittelem��n t�ss� 
n�kym�t toiminnallisesta n�k�kulmasta, �l� niink��n ajattele milt� ne n�ytt�v�t
- Aloitusn�kym�ss� on pelin logo, taustakuva ja kolme nappia joista p��st��n aloittamaan peli, s��t�m��n asetuksia ja katsomaan pisteit�.
- Pelin�kym�ss� on 2D karttan�kym� jossa n�kyv�t muut pelaajat ja vallattavat alueet eriv�risin�, alueiden valtauksen aikalaskuri sek� l�ydetyt "extrat" ja valikko josita ekstroja voi aktivoida. Lis�ksi n�kyy tiimikohtaiset pisteet jossain ruudun yl�reunassa.
- Peliasetukset-n�kym�st� l�ytyv�t peliasetukset, kuten pelaajien m��r�, laitteiden yhdist�minen peliin, valtausalueiden m��ritt�minen sek� er�n kesto ja pelimoodi.
- Pisten�kym�ss� n�kyv�t pelaajien pisteet sek� omat parhaat pisteet kautta aikojen.

4. M��rit� n�kymien v�liset siirtym�t korkealla tasolla, mist� n�kym�st� p��see minnekin? Mill� tavoin visualisoisit tilasiirtym�t?
Aloitusn�kym� (sis�lt�� valikon, taustakuvan ja pelin logon)
-> aloita peli -> peliasetukset -> pelin�kym�
-> liity peliin
-> profiili
-> pisteet

Pelin�kym� (2D pelikartta, tiimipisteet, ekstrat, oma ja muiden sijainti, valtausalueiden rajat, valikkoiconi josta p��see valikkoon)
->aloitusn�kym�
->omat asetukset

liity peliin (valittavissa olevat pelit, tietoa siit� mihin peliin on liittynyt sek� virhesanomat )
->pelin�kym�
->aloitusn�kym�

Profiili (oman hahmon nimi ja profiilikuva) 
-> pelin�kym��n jos peli on k�ynniss� tai aloitusn�kym��n

Pisteet (omat parhaat pisteet ja viimeisimpien pelien tiimipisteet) 
-> aloitusn�kym�

Tilasiirtymien v�liss� olisi 3Dzoom-fadein. Pelin k�ynnist�misen j�lkeen aloitusruutu ennen kuin peli lataa. Pelin loputtua loppuruutu jossa n�kyy voittanut tiimi ja kaikkien tiimien pisteet. Pelin�kymien v�liss� fade-to-black.

5. Listaa jokaista n�kym�� kohti tieto siit�, millaista tietosis�lt�� tai dataa k�ytt�liittym�ss� n�ytet��n.





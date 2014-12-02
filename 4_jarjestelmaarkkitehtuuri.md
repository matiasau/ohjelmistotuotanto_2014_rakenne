#  Järjestelmäarkkitehtuuri

* Pyri kuvailemaan tässä luvussa järjestelmäarkkitehtuuri yleisellä tasolla
* Mitä komponentteja järjestelmään tarvitaan jotta se pystyy palvelemaan määritettyjä käyttötapauksia?

## Käyttöliittymä
Mahdollistaa sovelluksen käytön pelin (pelimoottorin) ulkopuolella. Piirtää valikot ja mahdollistaa graafisen vuorovaikutuksen pelaajan ja ohjelman välillä.

## Autentikointi
Autentikointi tarkoittaa jokaisen pelaajan profiilin ja älylaitteen tunnistamista. Lisäksi tarvitaan jokaisen pelaajan profiilin tietojen tallennus pelaajan omaan älylaitteeseen paikalliseen tietokantaan josta tiedot voidaan pelin aikana ja lopussa hakea myös muiden pelaajien laitteisiin. Pelaajan profiiliin kuuluvat tiedot ovat nimi, profiilikuva ja parhaat henkilökohtaiset pisteet per peli.

## Sisätilapaikannus
Sisätilapaikannus toteutetaan käyttäen WLAN verkkoa. Kaikkien pelaajien täytyy olla samassa verkossa jotta peliä pystyy pelaamaan. Moduulin pitäisi osata sovelluksen käynnistyttyä etsiä lähellä olevia verkkoja ja tarjota pelaajalle valintaan automaattisesti vain ne verkot joissa on pelejä tarjolla. 

Ennen pelin alkua moduuli kalibroituu tarjolla olevan verkkosignaalin perusteella parhaan paikannustiedon takaamiseksi. Pelin käynnistyttyä moduuli paikantaa pelaajaa jatkuvasti ja syöttää sijaintidataa karttamoduulille sekä verkon kautta suojattuna muille pelaajille kyseisen pelaajan näyttämiseksi pelissä.

## Karttakomponentti
### Luotaessa uutta peliä
- mahdollistaa vektorimuotoisen tilakartan luomisen pelaajan inputin ja paikannustiedon perusteella
- karttaa voi halutessaan luoda useampi pelaaja jolloin peli saadaan nopeammin käyntiin
- mahdollistaa poweruppien lisäämisen tilakarttaan

### Pelin ollessa käynnissä
- hakee sisätilapaikannusmoduulilta jatkuvana datastriiminä paikallisen pelaajan sijantitiedot
- hakee verkosta jatkuvana datastriiminä muiden pelaajien paikannustiedot 
- käyttäjän aktiivisesta powerupista riippuen piilottaa pelaajan kartalta tai muuttaa pelaajan ikonia powerupin ehtojen mukaisesti

## Powerupit
Sisältää kaikki pelissä tarjolla olevat powerupit joita voi lisätä karttakomponentissa tilakarttaan ja sitä kautta peliin. Pelaajat voivat käyttää saamiaan poweruppeja missä tahansa pelin vaiheessa powerup-valikon kautta.
Esimerkkejä powerupeista:
- näkymättömyys 30 sekunniksi
- valloitustehokkuuden tuplaus
- toisen tiimin pisteet vähenevät X-määrällä

## Pelimoottori
Pelimoottori hallitsee eri moduulien sekä pelaajan ja pelin välistä vuorovaikutusta pelin aikana.

##### Pelimoottori
- piirtää (päivittää) karttakomponentin perusteella graafisesti kaikki pelaajat ja powerupit tilakartalle ikoneina,
- näyttää pelin tiedot, kuten tiimien pisteet numeroina ja graafisesti, 
- näyttää powerup-valikon, chatin ja päävalikon painikkeen

## Pelitietokanta
Jokaisen pelin tiedot tallennetaan peliin osallistuneiden käyttäjien älylaitteisiin paikalliseen tietokantaan josta tiedot ovat aina saatavissa tai kunnes pelaaja haluaa tiedot säilyttää. Tietokantaan tallennetaan seuraavia tietoja: tiimien parhaat pisteet, pelaajan parhaat pisteet, win/lose-ratio, peliaika, pelikartat sekä optionaalisesti pelaajien liikkeet pelin aikana. Viimeisin ominaisuus veisi mahdollisesti merkittävästi tilaa joten se olisi tästä syystä vaihtoehtoinen ja pelikohtainen.

## Chat
Mahdollistaa tiimikohtaisen ja reaaliaikaisen pelaajien vuorovaikuttamisen tekstiviesteillä pelin ollessa käynnissä.

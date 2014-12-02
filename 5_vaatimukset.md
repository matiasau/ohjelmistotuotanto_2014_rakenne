# Vaatimukset 

* Kuvaile tänne funktionaaliset ja ei-funktionaaliset vaatimukset
* Funktionaaliset vaatimukset
  * Tarkentavat käyttötapauksia
* Ei-funktionaaliset vaatimukset
  * Esim käytettävyyteen, tietoturvaan, tehokkuuteen, skaalautuvuuteen, hintaan ja prosessimalliin liittyvät vaatimukset
* **Muista esittää vaatimukset jäljitettävässä muodossa, yksiselitteisesti**
* Keskeinen tapa (erityisesti ei-funktionaalisiin vaatimuksiin) yksiselitteisille kuvauksille on vaatimusten **mitattavuus** (software metrics)

## Käyttöliittymä
Käyttöliittymän on oltava selkeä, helppokäyttöinen ja näyttävä. Sen on oltava yhdenmukainen pelin tyylin ja muun grafiikan kanssa.
Vaatimukset:
- käyttöliittymän täytyy täyttää [responsiivisen suunnittelun perusteet]
- enintään neljä suunnitteluväriä komponenteille ja tekstille
- fontin ja fonttikoon on oltava selkeää ja helppolukuista
- käyttöliittymän elementtien on oltava tarpeeksi suuria jotta niiden käyttö kosketusnäytöllä on helposti mahdollista
- käyttöliittymässä täytyy esiintyä pelin logo ja olla taustakuva

## Paikannus
Paikannuksen on toimittava tarpeeksi luotettavasti ja tarkasti jotta pelaaminen on mahdollista. Paikannuksen vaadittava tarkkuus hyvän pelikokemuksen mahdollistamiseksi on vähintään +-0,9m ja suositeltava tarkkuu +-0,75m pelaajan todellisesta lokaatiosta..

Paikallisen ja muiden pelaajien paikannustiedon hakemisen täytyy olla tarpeeksi nopeaa jotta pelikartta pystytään päivittämään tehokkaasti eikä lageja tai pelikokemusta huonontavia kokemuksia syntyisi. Pelikartan piirtonopeus ei saisi laskea milloinkaan alle 5fps:n.

## Turvallisuus
Tiedonsiirron täytyy olla turvattua esimerkiksi salauksen muodossa jotta ulkopuoliset, kolmannet osapuolet eivät pääsis tietoon käsiksi. Tähän tarkoitukseen voidaan käyttää yksinkertaista salausta. 

## Resurssien käyttö
Jokaisen pelaajan sijaintidata, poweruppien vaikutukset ja tiimien pisteet täytyy verkon kautta siirtää kaikille pelaajille mahdollisimman reaaliaikaisesti jotta pelikartan piirto olisi tehokkaasti mahdollista. Verkkoa ei saa pelidatalla ummettaa.

Pelikoodin täytyy olla optimoitua ja resurssien käytön tehokasta jotta peli toimisi hyvin mahdollisimman monella päätelaitteella.
- pelin täytyy käynnistyä millä tahansa päätelaitteella alle kahdessa (2) sekunnissa.
- pelitilassa ohjelman graafinen framerate ei saa tippua alle 20fps:n
- peli ei saa käyttää yli 60Mb välimuistia
- pelin täytyy mahtua alle 6Mb pakettiin

## Pelillisyys
Pelin on oltava hauska ja koukuttava. Se ei saa aiheuttaa pelaajalle negatiivista emootiota toimimattomuudella.

[responsiivisen suunnittelun perusteet]:http://digitaldesignstandards.com/standard/process/responsive-adaptive-design/


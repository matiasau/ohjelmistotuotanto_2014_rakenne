## Järjestelmän loppukäyttäjät

* Pelaaja voi toimia kahdessa eri roolissa:
	* *pelin ylläpitäjänä*, joka luo pelin ja liittyy siihen itsekin
	* *tavallisena pelaajana*, joka liittyy jo luotuun peliin

## Käyttötapauskaavio:

https://www.lucidchart.com/invitations/accept/375b9779-0afa-4e2b-baa9-0b7d403abaf4

## Tärkeimmät käyttötapaukset

#### 1) Uuden pelisession luominen ja pelaaminen:
__Alkutila:__ Sovellus käynnistyy aloitusvalikkoon.  
__Normaali kulku:__ Valitaan *Uusi peli*, määritetään pelisession asetukset, odotetaan peliin liittyviä muita pelaajia kunnes he ovat valmiita ja aloitetaan peli. Pelataan peliä, kunnes aikaraja tai pistetavoite on saavutettu.  
__Lopputila:__ tarkastellaan pisteitä, lopetetaan pelaaminen tai pelataan uusi peli.  
__Riskit:__ peliin ei liity muita pelaajia, jolloin peliä ei voi aloittaa.

#### 2) Valmiiseen pelisessioon liittyminen ja pelaaminen:
__Alkutila:__ Sovellus käynnistyy aloitusvalikkoon.  
__Normaali kulku:__ Valitaan *Liity peliin*, valitaan pelisessio jossa on tilaa, odotetaan peliin liittyviä muita pelaajia kunnes he ovat valmiita ja aloitetaan peli. Pelataan peliä, kunnes aikaraja tai pistetavoite on saavutettu.  
__Lopputila:__ tarkastellaan pisteitä, lopetetaan pelaaminen tai pelataan uusi peli.  
__Riskit:__ Ei löydy peliä, jossa olisi tilaa. Yhteys pelin ylläpitäjään (host) on heikko. 

#### 3) Oman profiilin asetuksien säätäminen
__Alkutila:__ Sovellus käynnistyy aloitusvalikkoon.  
__Normaali kulku:__ Valitaan *Profiili*, säädetään haluttuja asetuksia (nimimerkki, avatar, sosiaalinen media) koskettamalla niitä.  
__Lopputila:__ Palataan aloitusvalikkoon, jolloin tehdyt muutokset tallentuvat.  
__Riskit:__ Nimimerkki on jo jollain muulla pelaajalla käytössä. Avatarin pohjana käytettävä tiedosto on väärässä tiedostomuodossa tai liian suuri. Yhteys sovelluksen ulkopuolisiin sosiaalisen median palveluihin ei toimi.

#### 4) Parhaiden pisteiden ja muiden tilastojen tarkastelu
__Alkutila:__ Sovellus käynnistyy aloitusvalikkoon.  
__Normaali kulku:__ Valitaan *Pistetaulukko*, tarkastellaan pisteitä ja muita tilastoja halutuilla rajauksilla. Omissa tabeissaan on esimerkiksi *(a) viimeksi pelatut pelit*, *(b) parhaat tulokset halutulla aikavälillä*, *(c) henkilökohtaiset tulokset* ja *(d) tulokset joukkueittain*.   
__Lopputila:__ Palataan aloitusvalikkoon, kun pisteitä on tarkasteltu.  
__Riskit:__ -
 


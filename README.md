# Ilmiöt
# Alan toimintaympäristöt ja ilmiöt
Tekstiä voi kirjoittaa vaikka **lihavoituna**, *kursivoituna* tai ~~yliviivattuna~~   

Rivinvaihto tehdään kahdella välilyönnillä. 

Erilaisia otsikoita voi tehdä laittamalla # merkkejä peräkkäin:  
# 1. tason otsikko
## 2. tason otsikko
### 3. tason otsikko
#### 4. tason otsikko
##### 5. tason otsikko
###### 6. tason otsikko

Listoja voit tehdä näin: Eli tahdellä *
* Listan ensimmäinen elementti
* Listan toinen elementti
* Listan kolmas elementti
  * Kolmannen elementin ensimmäinen alielementti <!--Kaksi tabia sisennetty-->
  * Kolmannen elementin toinen alielementti
  
Numeroitu lista:
1. Eka juttu
1. Toka juttu
1. Kolmas juttu
   1. Kolmannen eka juttu <!--Kolme tabia sisennetty-->
   1. Kolmannen toka juttu
   
Readme.md -tiedostoon voi laittaa myös kuvia.
![Hyvinvointiteknologia](Lakki.jpg)


Linkitkin toimii:
http://google.com (automaattisesti)  
[Google](http://google.com)

Näinkin voi tehdä
> Kirjoitetaan tähän tekstiä  
> Tähän lisää tekstiä

Tässä tapauksessa teksti tulee laatikkoon, tätä käytetään usein koodin kirjoittamiseen Readme.md -tiedostossa:
````
function kirjoitaTeksti(kirjoita)
 if(kirjoita) {
  console.log("parametri oli tosi")
 }
````
Taulukon sarakkeen otsikko | Seuraavan sarakkeen otsikko
-------------------------|-----------------------
ABC | 123
XYZ | 456  

Voit myös kokeilla erilaisia emojeja :nerd_face: googlaa GitHub README.md emoji.   



# Sääaasema
## vaatimusmäärittely
### sovelluksen tarkoitus
* mitataan ympäristön lampötila -ja ilmankosteustietoja
* saatuja tietoja voidaan tarkastella tekstinä ja grafiikkana web sovelluksella

### käyttäjät
Web sovellus on tarkoitettu julkiseen käyttöön.

### käyttöliittymä
käyttöliittymä koostuu kahdesta näkymästä:
1. tekstimuotoisen datan selaamiseen tarkoitettu näkymä
1: grafiikkamuotoisen datan selaamiseen tarkoitettu näkymä

### jatkokehitysideoita
Säätietojen selaaminen valitulla aikavälillä.

## Arkkitehtuurikuvaus

### Luokkakaavio



### Sekvenssikaavio

## Työaikakirjanpito

päivä | aika | tehtävät
-----------|--------|-----
10.11 | 2h | Projektin suunnittelu
24.11 | 3h | Laitteiston asennus
25.11 | 2h| Ohjelmointi
01.12 | 5h | Testaaminen ja dokumentointi
08.12 | 9h | Käyttökoulutus
Yht | 28 | 

##  Käyttöohje

### Järjestelmän konfigurointi
Lataa node_modules

````
 npm install 

````
Käynnistä projekti paikallisesti portiin 3000

````
 npm start

````




//asetetaan oikeat pinnit

int led1 = D6;
int led2 = D7;

//kerrotaan pinneille että tarkoitus syöttää virtaa niihin.

void setup()
  {
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);

  }

//ja loopilla päättymättömästi toistaa virransyöttöä 1000 millisekunnin tauoilla.
void loop() 
  {
  digitalWrite (led1, HIGH);
  digitalWrite (led2, HIGH);

  delay(1000);

  digitalWrite (led1, LOW);
  digitalWrite (led1, LOW);

  delay (1000);

  }

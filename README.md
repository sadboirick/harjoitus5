# harjoitus5
Palvelinten Hallinta Harjoitus 5

Tässä raporttini Tero Karvisen Palvelinten Hallinta-kurssin tehtävästä 5. [Linkki tehtäviin.](http://terokarvinen.com/2018/aikataulu-%E2%80%93-palvelinten-hallinta-ict4tn022-4-ti-5-ke-5-loppukevat-2018-5p)

Käyttämäni tietokoneen speksit on:
- Emolevy: Asus Prime z270-K -emolevy
- Corsair Vengeance LPX DDR4 3000 MHz 16 Gt (2 x 8 Gt) -muistit
- Intel i5 7600k -prosessori
- 525 Gt Crucialin MX300 SSD
- Asus GeForce 1060 6GB DDR5 -näytönohjain
- Xubuntu 16.04.3 x64 livetikulta

[Oman Xubuntun saat ladattua täältä.](https://xubuntu.org/download/)

## Salt

Tehtävissä käytetään Salttia, eli asennetaan se

	sudo apt-get update
	sudo apt-get install -y salt-minion

## a) Valitse aihe omaksi kurssityöksi ja varaa se kommenttina aikataulusivun perään.

Valitsin aiheekseni Wordpressin ja siihen tarvittavan ympäristön asentamisen ja conffaamisen Saltilla. Tavoitteena saada wordpress pystyyn (ehkä jopa jonkun teeman kanssa) ilman että käyttäjän tarvitsisi ajaa Wordpressin omaa asennusskriptiä käsin.

## b) Julkaise raportti MarkDownilla. Jos käytät GitHub:ia, se tekee muotoilun automaattisesti “.md”-päätteisiin dokumentteihin.

Jes.

## c) Aja oma Salt-tila suoraa git-varastosta. Voit joko tehdä tilan alusta lähtien itse tai forkata sirottimen.

Väsätään nopea sls-tiedosto samaan git varastoon, mihin tehtäväkin tehdään. Nimetään se top.sls, jotta sen voi ajaa komennolla

	sudo salt-call --local state.highstate --file-root .



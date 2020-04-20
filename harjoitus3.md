#Harjoitus 3 - Versionhallinta

	#a) MarkDown. Tehdään tämän tehtävän raportti MarkDownina.

	Aluksi tehdään käyttäjä GitHubiin, ja lisätään uusi repository tässä tapauksessa nimeltä
	harjoitus3. Valitsin myös suositellun "GNU General Public License v3.0" lisenssiksi.

	Seuraavaksi asensin Gitin $ sudo apt-get -y install git , ja kloonasin äsken tehdyn repositoryn
	ensin kopioimalla repositoryn osoitteen GitHubista ja syöttämällä komennon 
	$ git clone https://github.com/KiljuLasse/harjoitus3.git

	Asennuksen jälkeen siirryin asennettuun kohteeseen ja loin MarkDown -tiedoston nimeltä
	harjoitus3 $ sudo nano harjoitus3.md

	Tiedoston luotua tallensin sen ja synkronoin tehdyt muutokset GitHubiin
	$ git add harjoitus3.md && git commit; git pull && git push ja seurasin annettuja ohjeita.

	Testasin vielä, että muutokset tulevat myös GitHubiin.

	#d) Näytä esimerkit kommennoista 'git log', 'git diff' ja 'git blame'

	$ git log

	Tämä komento kertoo kuka on tehnyt muutoksia, milloin ja mikä oli kommentti muutosta tehtäessä.
	Näyttää siis toisin sanoen logit commitista.

	$ git diff

	Komento näyttää mihin tiedotoihin on tehty muutoksia ja listaa kuinka paljon muutoksia on tehty
	+ ja - merkeillä. Listaa alle myös poistetut ja lisätyt muutokset kokonaisuutena.

	$ git blame

	Komento listaa kuka on muokannut viimeksi tiettyä kohtaa halutusta tiedostosta. Tässä tapauksessa
	$ git blame /home/lasse/harjoitus3/harjoitus3.md

	#e) Tee tyhmä muutos gittiin.

	Luodaan ensin uusi tiedosto nimeltä tyhma $ sudo nano tyhma
	Kirjoitetaan tiedostoon ensin "fiksua tekstia" ja tallennetaan tiedosto.
	Lisätään tehdyt muutokset $ git add tyhma.txt ja $ git commit
	Tarkistetaan vielä muutokset käyttämällä $ git log

	Seuraavaksi mennään lisäämään "tyhma" tiedostoon teksti "tyhmaa tekstiä" ja ei tehdä committia.
	Tehdään $ git reset --hard ja huomataan, että teksti "tyhmaa tekstia" on kadonnut tiedostosta
	ja jäljelle on jäänyt vain "fiksua tekstia" mikä commitattiin. Reset tehtiin siis viimeisimpään
	committiin, eli vain fiksu teksti jäi jäljelle.

	

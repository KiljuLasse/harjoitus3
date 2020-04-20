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

	Tämä

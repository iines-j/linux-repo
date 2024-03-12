Kurssin päätöksenä tehty [Final Lab.](https://terokarvinen.com/2024/arvioitava-laboratorioharjoitus-2024-linux-palvelimet/)
Aloitettu klo 10.20 ja loppui klo 13.00.
____
## c) Ei kolmea sekoseiskaa
> Suojaa raportti Linux-oikeuksilla niin, että vain oma käyttäjäsi pystyy katselemaan raporttia.

<img src="https://github.com/iines-j/linux-repo/assets/148907657/f6a8b871-f07d-4ff7-b04a-9e15f867ca84" width="600"></img> 

## d) 'howdy'
> Tee kaikkien käyttäjien käyttöön komento 'howdy'.
> - Tulosta haluamaasi ajankohtaista tietoa, esim päivämäärä, koneen osoite tms.
> - Pelkkä "hei maailma" ei riitä.
> -  Komennon tulee toimia kaikilla käyttäjillä työhakemistosta riippumatta.

Epähuomiossa en nimennyt komentoa aluksi 'howdy'ksi, joten uudelleennimesin sen ja laitoin uudestaan kaikkien käyttöön.

<img src="https://github.com/iines-j/linux-repo/assets/148907657/729b3bf5-1d88-4f58-9fb2-d888fd45161f" width="600"></img>
<img src="https://github.com/iines-j/linux-repo/assets/148907657/876e6463-e2df-4cbc-b849-91a09c56ead3" width="600"></img>


## e) AI kakone
>  Asenna Apache-weppipalvelin.
> - Tee yrityksellemme "AI Kakone" kotisivu. Kotisivu tulee näkyä koneesi IP-osoitteella suoraan etusivulla.
> - Sivua pitää päästä muokkaamaan normaalin käyttäjän oikeuksin (ilman sudoa).
> - Liitä raporttiisi listaus tarvittavien tiedostojen ja kansioiden oikeuksista.

Tiedostot & kansiot ja niiden oikeudet:
```
-rw-r--r-- 1 root root  172 12. 3. 10:44 aikakone.conf
drwxr-xr-x 3 lab-iines lab-iines 4096 12. 3. 10:45 publicsites
drwxr-xr-x 2 lab-iines lab-iines 4096 12. 3. 10:48 aikakone 
-rw-r--r-- 1 lab-iines lab-iines 10 12. 3. 10:48 index.html 
```

<img src="https://github.com/iines-j/linux-repo/assets/148907657/a0a3d799-ed90-4383-8743-709d268d8131" width="600"></img> 

## g) ssh
> Asenna ssh-palvelin.
> - Tee uusi käyttäjä omalla nimelläsi, esim. minä tekisin "Tero Karvinen test", login name: "terote01".
> - Automatisoi ssh-kirjautuminen julkisen avaimen menetelmällä, niin että et tarvitse salasanoja, kun kirjaudut sisään.
> - Voit käyttää kirjautumiseen localhost-osoitetta.

- user: iineste01 
- ssh toimii ilman salasanaa

<img src="https://github.com/iines-j/linux-repo/assets/148907657/37c0cc6a-f846-41ee-ae16-74a668258d2a" width="600"></img> 
<img src="https://github.com/iines-j/linux-repo/assets/148907657/e5c06147-03b0-4633-b279-3c9b76654990" width="600"></img> 

## h) Django
> Asenna omalle käyttäjällesi Django-kehitysympäristö. <br/>
> Tee tietokantaan lista tekoälyistämme, jossa on nämä ominaisuudet
>  - Kirjautuminen salasanalla
>  - Tietokannan muokkaus wepissä Djangon omalla ylläpitoliittymällä (Django admin)
>  - Käyttäjä Erkille, jossa ei ole ylläpito-oikeuksia
>  - Taulu Assistants, jossa jokaisella tietueella on nimi (name)
>  - Jos haluat, voit lisäksi bonuksena laittaa mukaan kentän koko (size)

- superuser: admin
- user: erkki 

<img src="https://github.com/iines-j/linux-repo/assets/148907657/54c4c653-7d82-498f-b99d-86b8cd0ad2d0" width="600"></img> 
<img src="https://github.com/iines-j/linux-repo/assets/148907657/443d49f4-7408-4d39-b1bf-215913ec0b7f" width="600"></img> 
 
Huomasin vasta tehtävän tehtyä että nimesin kansion tyhmästi publicwsgi:ksi, kun sinne tosiaan laitoin ton dev-version djangosta. <br/>
Joten sen tuotantoversion laitankin nyt django-kansioon. 

## h) Bonus: Djangon tuotantoasennus
> Tee tuotantotyyppinen asennus Djangosta.
> - Laita Django-lahjatietokanta tuotantotyyppiseen asennukseen
> - Voit vaihtaa tämän sivun näkymään etusivulla staattisen sivun sijasta

- toimii suoraan localhostissa

 <img src="https://github.com/iines-j/linux-repo/assets/148907657/e7ef4b40-327b-4ac0-a26f-a998e9a9ec02" width="600"></img> 
___
## Lähteet
- Tero Karvinen. Final Lab for Linux Palvelimet 2024 Spring. [Linkki.](https://terokarvinen.com/2024/arvioitava-laboratorioharjoitus-2024-linux-palvelimet/) Luettu 12.3.2024.

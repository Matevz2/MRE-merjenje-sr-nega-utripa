# MRE-merjenje-srčnega-utripa
Projekt,ki ga imava jaz in moj sošolec pri predmetu MRE. Naredila bova merilnik srčnega utripa z senzorjem MAX30102. Uporabila bova tudi arduino nano, OLED display in stikalo 

### Opis delovanja projekta
Naprava je namenjena merjenju srčnega utripa in nasičenosti krvi s kisikom (SpO2). Temelji na senzorju MAX30102, ki za svoje delovanje uporablja rdečo in infrardečo LED diodo ter fotodetektor. Senzor zaznava spremembe v pretoku krvi skozi prst uporabnika. Ob vsakem srčnem utripu se količina krvi v žilah rahlo spremeni, kar povzroči spremembo absorpcije svetlobe. Te spremembe senzor pretvori v električni signal.

Ko uporabnik položi prst na senzor, Arduino Nano začne brati podatke in jih obdelovati. Program filtrira šum in iz pridobljenih podatkov izračuna srčni utrip v udarcih na minuto (BPM). Poleg tega senzor omogoča tudi oceno nasičenosti krvi s kisikom, kar predstavlja pomemben podatek o delovanju krvnega obtoka in dihalnega sistema.

Izračunane vrednosti se nato prikažejo na OLED zaslonu, ki uporabniku omogoča hitro in enostavno odčitavanje rezultatov. Zaradi majhne porabe energije in kompaktne izvedbe je naprava primerna za uporabo doma, v šoli ali pri demonstraciji osnov delovanja biometričnih senzorjev.

### Kosovnica uporabljenih materialov in komponent
<img width="1067" height="343" alt="image" src="https://github.com/user-attachments/assets/29ed831a-dba8-4283-bad7-c353fac5d714" />


### Slika vezalne sheme
<img width="972" height="653" alt="image" src="https://github.com/user-attachments/assets/f073a34e-f927-4926-afd2-4814339079a2" />

### Slike načrtov za ohišje 

### Izračune za posamezne komponente elektronskega vezja
Ker projekt temelji predvsem na digitalnih komponentah z že vgrajeno elektroniko, ni bilo potrebno izvajati zahtevnejših električnih izračunov. Komponente delujejo pri napetosti 3,3 V oziroma 5 V, ki jo zagotavlja Arduino Nano.

Poraba toka senzorja MAX30102 je relativno majhna in je primerna za napajanje neposredno iz mikrokontrolnika. OLED zaslon prav tako ne zahteva dodatnih močnostnih elementov. Zaradi tega v vezju niso bili potrebni upori za omejevanje toka, tranzistorji ali releji.

### Koda programa
Koda se nahaja v
mapi po imenu koda 

### Videoposnetek delovanja naprave

### A-test

### Komentar in ocena natančnosti
Med razvojem projekta sva izvedla več primerjalnih meritev z referenčnim pulznim oksimetrom. Cilj je bil ugotoviti, kako natančno senzor MAX30102 meri srčni utrip in nasičenost krvi s kisikom.

Rezultati so pokazali, da so bile meritve srčnega utripa večinoma zelo podobne referenčni napravi. Največja odstopanja so se pojavila ob premikanju prsta ali nepravilni namestitvi na senzor. Pri meritvah nasičenosti krvi s kisikom so bila začetna odstopanja nekoliko večja, vendar so se po prilagoditvah programske kode bistveno zmanjšala.

Ugotovila sva, da na natančnost meritev vplivajo predvsem kakovost stika med prstom in senzorjem, količina zunanje svetlobe ter mirnost uporabnika med meritvijo. Kljub določenim omejitvam so bile končne meritve dovolj natančne za prikaz delovanja sistem

### Predlagane izboljšave in kalibracija senzorja 
V prihodnje bi lahko projekt nadgradila na več načinov. Ena od možnosti je uporaba kakovostnejšega medicinskega senzorja, ki bi omogočal še bolj natančne meritve. Prav tako bi lahko uporabila večji OLED ali LCD zaslon, na katerem bi bilo mogoče prikazati dodatne informacije.

Naslednja izboljšava bi bila dodajanje brezžične povezave Bluetooth ali Wi-Fi. Tako bi lahko meritve pošiljali na mobilni telefon ali računalnik ter jih shranjevali za kasnejšo analizo.

Nadgradnja bi bila tudi izdelava aplikacije za spremljanje zdravstvenih podatkov. Aplikacija bi uporabniku omogočala pregled zgodovine meritev, grafični prikaz rezultatov in opozorila ob nenavadnih vrednostih.

Kalibracijo senzorja sva izvedla s primerjavo rezultatov z referenčnim pulznim oksimetrom. Na podlagi primerjalnih meritev sva prilagodila programsko kodo in izboljšala stabilnost prikazanih vrednosti. Za še večjo natančnost bi bilo potrebno opraviti dodatne meritve na več uporabnikih ter pripraviti natančnejšo kalibracijsko metodo.

### Zaključek
Projekt je bil uspešno izveden in je dosegel zastavljene cilje. Izdelala sva delujočo napravo za merjenje srčnega utripa in nasičenosti krvi s kisikom z uporabo senzorja MAX30102, Arduino Nano mikrokrmilnika in OLED zaslona.

Med izdelavo sva pridobila veliko praktičnega znanja s področja elektronike, programiranja mikrokontrolnikov in obdelave podatkov senzorjev. Spoznala sva tudi delovanje komunikacijskega protokola I2C ter načine prikaza podatkov na zaslonu.

Kljub nekaterim težavam med razvojem sva uspešno odpravila večino napak in izboljšala delovanje sistema. Končna naprava deluje stabilno, meritve pa so primerljive z referenčnimi napravami.

Projekt predstavlja dobro osnovo za nadaljnji razvoj. Z dodatnimi izboljšavami bi bilo mogoče izdelati še natančnejšo in uporabniku prijaznejšo napravo za spremljanje osnovnih zdravstvenih parametrov.


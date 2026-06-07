# MRE-merjenje-srčnega-utripa
Projekt,ki ga imava jaz in moj sošolec pri predmetu MRE. Naredila bova merilnik srčnega utripa z senzorjem MAX30102. Uporabila bova tudi arduino nano, OLED display in stikalo 

### Opis delovanja projekta
Naprava je namenjena merjenju srčnega utripa uporabnika. Deluje s pomočjo senzorja MAX30102, ki uporablja rdečo in infrardečo svetlobo za zaznavanje sprememb pretoka krvi v prstu. Ko uporabnik položi prst na senzor,ta nekaj časa meri in potem pošlje podatke Arduinu. Zelo pomembnoje da se prst ne premika in da je senzor v temu, če ne bodo meritve drugačne. Iz sprememb signala mikrokrmilnik Arduino Nano izračuna srčni utrip v udarcih na minuto (BPM) in jih prikaže na OLED displayu.
Stikalo sva dodala,da lahko napravo izklopimo, ko ni uporabljena. Ko je naprava vključena, Arduino bere podatke iz senzorja in jih prikazuje preko zaslona. Sistem je primeren za osnovno spremljanje srčnega utripa, dodala pa sva še nekaj. In sicer odstotek kisika, ki ga hemoglobin prenaša v vaši krvi  SpO2 (saturacija s kisikom).

### Kosovnica uporabljenih materialov in komponent
<img width="1524" height="585" alt="image" src="https://github.com/user-attachments/assets/3d95dfeb-eae3-4fdf-8a4e-fb492561ed5e" />

### Slika vezalne sheme
<img width="972" height="653" alt="image" src="https://github.com/user-attachments/assets/f073a34e-f927-4926-afd2-4814339079a2" />

### Slike načrtov za ohišje 

### Izračune za posamezne komponente elektronskega vezja
Za projekt nisva delala nobenih izračunov, ker nisva uporabljala nobenih uporov, tranzistorjov, relejev...

### Koda programa

### Videoposnetek delovanja naprave

### A-test

### Komentar in ocena natančnosti

### Predlagane izboljšave 

### Zaključek


# Autor: Piotr Smęt
# Przebieg procesu budowania pakietu

Zdecydowano się na pakiet `GNU time`.

## 1. Pobranie plików źródłowych {#pobranie-plików-źródłowych .unnumbered}

Polecenie: `sudo apt-get source time`

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 192243.png" style="width:90.0%" />
<figcaption>Pobieranie plików źródłowych.</figcaption>
</figure>

## 2. Pobieranie zależności {#pobieranie-zależności .unnumbered}

Polecenie: `sudo apt-get build-dep time`

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 192357.png" style="width:90.0%" />
<figcaption>Rozpoczęcie pobierania zależności.</figcaption>
</figure>

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 192412.png" style="width:90.0%" />
<figcaption>Zakończenie instalacji zależności.</figcaption>
</figure>

## 3. Budowanie pakietu {#budowanie-pakietu .unnumbered}

Polecenie: `sudo debuild -b -uc -us`

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 192736.png" style="width:90.0%" />
<figcaption>Rozpoczęcie budowania pakietu.</figcaption>
</figure>

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 192803.png" style="width:90.0%" />
<figcaption>Zakończenie budowania pakietu - wygenerowanie pliku
.deb.</figcaption>
</figure>

# Instalacja i uruchomienie programu

## 1. Instalacja pakietu {#instalacja-pakietu .unnumbered}

Polecenie: `sudo dpkg -i time_1.9-0.1build2_amd64.deb`

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 193138.png" style="width:90.0%" />
<figcaption>Instalacja zbudowanego pakietu deb.</figcaption>
</figure>

## 2. Uruchomienie programu {#uruchomienie-programu .unnumbered}

Polecenie: `\time -v pwd`

<figure data-latex-placement="H">
<img src="./Zrzut ekranu 2026-05-30 193410.png" style="width:90.0%" />
<figcaption>Uruchomienie programu i pomiar czasu wykonania.</figcaption>
</figure>

# Wnioski

Proces budowania pakietu ze źródeł przebiegł bezproblemowo i przyjemnie.

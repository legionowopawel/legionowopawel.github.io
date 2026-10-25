# Pamiętliwy przeciwnik

Zręcznościowa gra przeglądarkowa, w której przeciwnik uczy się z tego, gdzie lubisz stać, i właśnie tam uderza.

## Pomysł

Większość gier ma przeciwnika, który działa według stałego schematu. Tutaj jest odwrotnie: to Ty jesteś dla niego wzorem do nauki. Im dłużej stoisz w jednym miejscu, tym lepiej Cię zna i tym celniej strzela. Wygrywa ten, kto potrafi być nieprzewidywalny.

## Cel gry

Przetrwaj jak najdłużej. Masz **3 życia**, a wynik to czas przetrwania w sekundach. Najlepszy wynik jest zapamiętywany w trakcie sesji.

## Zasady

1. Poruszasz się po kwadratowej arenie podzielonej na siatkę 14 × 14 pól.
2. Gra zapisuje, ile czasu spędzasz w każdym polu (a trochę także w sąsiednich). To jest „pamięć” przeciwnika.
3. Co jakiś czas przeciwnik wybiera cel, losując pole z prawdopodobieństwem rosnącym wraz z Twoim czasem pobytu w nim.
4. Cel jest oznaczany **czerwonym kołem ostrzegawczym**, które się wypełnia.
5. Gdy koło się wypełni, następuje wybuch. Jeśli jesteś w jego zasięgu, tracisz życie.
6. Po trafieniu masz krótką nietykalność (około 1,2 s), podczas której postać miga.
7. Starsze dane w pamięci przeciwnika stopniowo wygasają, więc zmiana nawyków naprawdę pomaga.

## Rosnący poziom trudności

- Uderzenia są coraz częstsze.
- Czas ostrzeżenia się skraca (od ok. 1,1 s do 0,6 s).
- Co ok. 25 sekund dochodzi kolejne równoległe uderzenie (maksymalnie 4 naraz).
- Co jakiś czas przeciwnik strzela w losowe miejsce, więc nie da się go całkowicie przechytrzyć jednym trikiem.

## Sterowanie

| Platforma | Ruch | Start / restart |
|---|---|---|
| Komputer | strzałki lub WASD | spacja lub Enter |
| Telefon / tablet | przeciąganie palcem po planszy | dotknięcie planszy |

## Interfejs

- **Czas** i **liczba żyć** wyświetlane w górnych rogach planszy.
- **Mapa cieplna**: czerwone podświetlenie pól pokazuje, co przeciwnik o Tobie „wie”. Przycisk pod planszą pozwala ją pokazać lub ukryć. Bez niej gra jest trudniejsza.
- Ekran końcowy z czasem, liczbą trafień i rekordem.

## Wskazówki

- Nie stój w miejscu dłużej niż kilka sekund.
- Unikaj własnych schematów, na przykład krążenia po okręgu. Przeciwnik też je zapamięta.
- Dobrze działa nagła zmiana strefy: dane o starym miejscu wygasają, a nowe dopiero się buduje.
- Włącz mapę cieplną, żeby zobaczyć, jak Twoje nawyki zamieniają się w cel.

## Dane techniczne

- Jeden plik HTML z wbudowanym CSS i JavaScriptem, bez zewnętrznych zależności.
- Rysowanie na elemencie `<canvas>`, pętla oparta na `requestAnimationFrame`.
- Obsługa klawiatury, myszy i dotyku.
- Jasny i ciemny motyw strony zgodnie z ustawieniami systemu.

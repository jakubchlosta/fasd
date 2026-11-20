# Biblioteka gier steam - zbiór danych w formatach xml, json, csv

---

Repozytorium zawiera zbiór danych przedstawiajacy wybrane gry z mojej biblioteki **Steam**.



## Zawartość repozytorium

* 'steam-lib.xml' - dane zapisane w jezyku znacznikow XML.
* 'steam-lib.xsd' - schemal XML definiujacy strukture, typy danych i ograniczenia dla pliku XML.
* 'steam-lib.json' - ten sam zestaw gier zapisany w formacie JSON.
* 'steam-lib.csv' - dane zapisane w formiacie CSV.
* 'README.md' - opis repozytorium.

---

## Jak czytać dane?

'id' - unikalny numer gry.

'title' - Tytuł gry

'developer' - Twórca / studio deweloperskie.

'releaseYear' - rok wyjścia gry.

'purchaseDate' - data zakupu (RRRR.MM.DD).

'sizeGB' - rozmiar gry w GB.

'hoursplayed' - ilosc godzin w grze.

'tags' - tagi opisujące gre.

---

## Różnice miedzy wybranymi formatami



### XML + XSD
* **Budowa drzewiasta:** Podobnie jak w HTML, w XML uzywamy znacznikow. Tagi są zagnieżdzone w osobnym bloku.
*  **Minusy:** ze wzgledu na jego budowe, jest to zajmujący najwiecej linii format.

### JSON
* **Budowa:** zamiast znacznikow, uzywamy nawiasow klamrowych dla obiektow i nawiasow kwadratowych dla list.
* **Czytelność:** JSON zdecydowanie jest najczytelniejszym formatem.

### CSV
* **Budowa:** pierwsza linijka to nazwa kolumn, a kazdy kolejny wiersz to jedna gra. Wszystkie wartości są oddzielone przecinkiem ",".
*  **Minusy:** brak tablic. Przez co wszystkie tagi są oddzielone średnikiem ";". Brak typów danych.

---

## Sprawdzanie poprawności plików

Pliki zostały utworzone w edytorze Visual Studio Code.

1. **XML** został sprawdzony wzgledem schematu **XSD** za pomocą rozszerzenia *XML* od Red Hat.
2. **JSON** został sprawdzony wbudowanym walidatorem w VS Code.
3.  **CSV** został sprawdzony pod kątem równej liczby kolumn w każdym wierszu za pomocą rozszerzenia *Rainbow CSV*.
  
---

Linki użyte przy nauce składni:
* https://www.w3schools.com/xml/schema_intro.asp
* https://www.w3schools.com/xml/
* https://www.w3schools.com/js/js_json.asp
* https://pl.wikipedia.org/wiki/CSV_(format_pliku)
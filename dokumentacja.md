# dokumentacja testow jednostkowych w c# dla aplikacji wpf (xaml)

1. **wstep**
   - ***testy jednostkowe*** to kluczowy element w procesie tworzenia oprogramowania, ktory zapewnia, ze poszczegolne czesci kodu dzialaja zgodnie z oczekiwaniami
   - ***xunit*** to darmowe, otwarte, zorientowane na spolecznosc narzedzie do testowania jednostek dla .net framework, sluzy do do testowania jednostek c#, f#, vb.net i innych jezykow .net

2. **tworzenie projektu testowego**
   - ***aby dodac nowy projekt testowy w visual studio*** nalezy otworzyc rozwiazanie ktore zawiera kod ktory chcemy przetestowac, potem prawym przyciskiem myszki kliknac *rozwiazanie* w *eksplorator rozwiazan* i wybrac polecenie *dodaj nowy projekt* a potem kliknac *szablon projektu testow jednostkowych*

3. **instalacja niezbednych bibliotek**
   - ***instrukcje instalacji pakietow nuget***<br>
     dodaje lub aktualizuje xunit
     ```sh
     dotnet add package xunit
     ```
      dodaje lub aktualizuje xunit do visual studio
      ```sh
     dotnet add package xunit.runner.visualstudio
       ```
      dodje lub aktualizuje pakiet ktory ulatwia projekty testowe
      ```sh
     dotnet add package Microsoft.NET.Test.Sdk
       ```
4. **uruchamianie testow**
   - aby **uruchomic test** w konsoli polecen nalezy uzyc polecenia
     ```sh
     dotnet.test
     ```
     -w visual studio nalezy uzyc *eksploratora testow*

5. **najczęstsze bledy i sposoby ich rozwiązania**
   - ***aby zaimplementowac inotifypropertychanged*** nalezy zadeklarowac zdarzenie *propertychanged* i stworzyc metode *onpropertychanged*. potem dla kazdej wlasciwosci dla ktorej chcesz zmienic powiadomienia nalezy wywolac *onpropertychanged* za kazdym razem gdy zostanie zaktualizowana

<!--4. **pisanie testow jednostkowych**
   - *Testowanie klasy biznesowej (np. obliczanie wartości podatku).*
   - *Sprawdzanie poprawności **INotifyPropertyChanged**.*
   - *Obsługa wyjątków i przypadków brzegowych.*
-->

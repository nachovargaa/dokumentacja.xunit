# Dokumentacja testów jednostkowych w C# dla aplikacji WPF (XAML)

1. **Wstęp**
   - ***testy jednostkowe*** to kluczowy element w procesie tworzenia oprogramowania, ktory zapewnia, ze poszczegolne czesci kodu dzialaja zgodnie z oczekiwaniami
   - ***xunit*** to darmowe, otwarte, zorientowane na spolecznosc narzedzie do testowania jednostek dla .net framework, sluzy do do testowania jednostek c#, f#, vb.net i innych jezykow .net

2. **Tworzenie projektu testowego**
   - ***aby dodac nowy projekt testowy w visual studio*** nalezy otworzyc rozwiazanie ktore zawiera kod ktory chcemy przetestowac, potem prawym przyciskiem myszki kliknac *rozwiazanie* w *eksplorator rozwiazan* i wybrac polecenie *dodaj nowy projekt* a potem kliknac *szablon projektu testow jednostkowych*
   - *Konfiguracja frameworka testowego i dodanie referencji do głównego projektu.*

3. **Instalacja niezbędnych bibliotek**
   - *Instrukcje instalacji pakietów NuGet:*
     ```sh
     dotnet add package xunit
     dotnet add package xunit.runner.visualstudio
     dotnet add package Microsoft.NET.Test.Sdk
     ```

4. **Pisanie testów jednostkowych**
   - *Testowanie klasy biznesowej (np. obliczanie wartości podatku).*
   - *Sprawdzanie poprawności **INotifyPropertyChanged**.*
   - *Obsługa wyjątków i przypadków brzegowych.*

5. **Uruchamianie testów**
   - ***Visual Studio**: Test Explorer.*
   - ***Terminal**:*  
     ```sh
     dotnet test
     ```

6. **Najczęstsze błędy i sposoby ich rozwiązania**
   - *Problemy z wersją frameworka `.NET 8.0` vs `net8.0-windows`.*
   - *Obsługa `PropertyChanged` i poprawne implementowanie `INotifyPropertyChanged`.*

Część 1: Tworzenie Struktury i Inicjalizacja

Opis:

Ta część kodu koncentruje się na definicji i inicjalizacji podstawowych struktur danych oraz przygotowaniu niezbędnych funkcji pomocniczych.

	1.	Inicjalizacja pracowników:
	•	Funkcja utworzPracownikow inicjalizuje tablicę pracowników. Ustawia ich identyfikatory, imiona, dostępność oraz początkowe wartości liczników rozmów i czasu rozmowy.
	2.	Generowanie losowych danych:
	•	Funkcja DlugoscPolaczen generuje losową długość połączenia telefonicznego na podstawie rozkładu normalnego.
	•	Funkcja PrzychodzacePolaczenia generuje losową liczbę przychodzących połączeń na podstawie rozkładu Poissona.
	3.	Operacje na kolejce:
	•	Funkcja DodajDoKolejki dodaje nowy element na koniec kolejki.
	•	Funkcja UsunElementZPoczatkuKolejki usuwa element z początku kolejki.
	•	Funkcja WypiszKolejke wypisuje całą zawartość kolejki.
	•	Funkcja DlugoscKolejki zwraca długość kolejki.

Część 2: Obsługa Połączeń i Symulacja

Opis:

W tej części skupiamy się na logice obsługi połączeń telefonicznych oraz przeprowadzeniu symulacji.

	1.	Obsługa połączeń:
	•	Funkcja ObslugaPolaczen generuje przychodzące połączenia i przypisuje klientów do dostępnych pracowników. Jeśli nie ma dostępnych pracowników, dodaje klientów do kolejki.
	2.	Sprawdzanie statusu pracowników:
	•	Funkcja SprawdzPracownikow sprawdza, czy pracownicy zakończyli rozmowy i aktualizuje ich status. Przypisuje również klientów z kolejki do wolnych pracowników.
	3.	Symulacja:
	•	Funkcja Symulacja przeprowadza symulację działania centrali telefonicznej przez określony czas (8 godzin, podzielonych na 15-minutowe interwały). W każdym interwale obsługuje połączenia, aktualizuje czas rozmów i przypisuje klientów z kolejki.

Część 3: Interfejs Użytkownika i Start Programu

Opis:

Ta część kodu odpowiada za interfejs użytkownika i uruchomienie programu.

	1.	Tekst startowy:
	•	Funkcja tekst_startowy obsługuje główne menu programu. Umożliwia użytkownikowi wybór między rozpoczęciem symulacji, wyświetleniem listy pracowników oraz wyjściem z programu.
	2.	Interakcje użytkownika:
	•	Funkcja zapewnia, że użytkownik wprowadza prawidłowe dane i odpowiednio reaguje na jego wybory. W przypadku wyboru opcji wyświetlenia listy pracowników, wyświetla ich imiona.
	3.	Główna funkcja programu:
	•	Funkcja main inicjalizuje losowy generator liczb, tworzy pracowników i uruchamia główny interfejs użytkownika.

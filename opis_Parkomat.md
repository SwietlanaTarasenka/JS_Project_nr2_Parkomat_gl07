# JS_Project_nr2_Parkomat_gl07
Temat projektu nr 2. Program, realizujący działanie parkomatu.

Link: 

Opis zadania.

-Parkomat przechowuje informacje o monetach/banknotach znajdujacych sie w nim (1, 2, 5, 10, 20, 50gr, 1, 2, 5, 10, 20, 50 zł).

-Okno z polem tekstowym na numer rejestracyjny pojazdu, aktualną datę (rok, miesiąc, dzień, godzina, minuta), 
data wyjazdu z parkingu (rok, miesiąc, dzień, godzina, minuta), przyciskami pozwalającymi na wrzucanie monet (prosze umiescic pole
pozwalajace wpisać liczbe wrzucanych monet), oraz przyciskiem “Zatwierdz’.

-Program powinien zawierac pole pozwalajace na przestawienie aktualnego czasu.

-Zasady strefy parkowania:

  +Strefa platnego parkowania obowigzuje w godzinach od 8 do 20 od poniedziatku do piatku.
  
  +Pierwsza godzina ptatna 2 zł.
  
  +Druga godzina platna 4 zł.
  
  +Trzecia i kolejne godziny ptatne po 5 zł.
  
  +Czas wychodzacy poza obowiazywanie platnego parkowania przechodzi na kolejny dzien  
  
      -Wykupienie godziny parkowania o 19:20 w pigtek pozwala na parkowanie do
        8:20 w poniedziatek (koniec 0 20:20, wychodzi 20 minut poza ptatne
        parkowanie, przechodzi na kolejny ptatny dzien).
        
-Po kazdym wrzuceniu monety termin wyjazdu aktualizuje sie zgodnie z cala wrzuconą kwota.

-Jesli wrzucone zostato mniej pieniedzy niz potrzeba na opłacenie pełnej godziny, to opłacana jest niepełna godzina:

  +Wrzucenie  1zł pozwala na parkowanie 30 minut,
  +Wrzucenie 5 zł pozwala na parkowanie 1 godzine i 45 minut (2 zł na opłacenie pierwszej godziny, 
    zostato 3zł, a potrzeba 4zł na oplacenie kolejnej, co daje 3/4 godziny: 45 minut).
    
-Po wcisnieciu przycisku “Zatwierdz” wyswietlane jest okno z potwierdzeniem
opłacenia parkingu: numer rejestracyjny pojazdu, czas zakupu i termin wyjazdu.

-Numer rejestracyjny moze skladać sie tylko z dużych liter od A do Z i cyfr.

-W automacie miesci sie dowolna liczba banknotów (10, 20, 50 zł) i po 200 monet
kazdego rodzaju. Próba wrzucenia monety ponad limit powoduje wyswietlenie
informacji o przepełnieniu parkomatu i prosbe o wrzucenie innego nominału.

Testy.

1. Ustaw niepoprawna godzine. Oczekiwany komunikat o błedzie. Ustawić godzine na 12:34.
2. Wrzucić 2 zł, oczekiwany termin wyjazdu godzine po aktualnym czasie. Dorzuc
4zł, oczekiwany termin wyjazdu dwie godziny po aktualnym czasie. Dorzuć 5 zł,
oczekiwany termin wyjazdu trzy godziny po aktualnym czasie. Dorzué kolejne 5 zł,
oczekiwany termin wyjazdu cztery godziny po aktualnym czasie.
3. Wrzucic tyle pieniedzy, aby termin wyjazdu przeszedł na kolejny dzien, Zgodnie z
zasadami-- wrzucic tyle monet aby termin wyjazdu był po godzinie 19:00,
dorzucić monete 5 zł,
SC ONO
4. Wrzucic tyle pieniedzy, aby termin wyjazdu przeszedł na kolejny tydzien, zgodnie z
zasadami- wrzucic tyle monet aby termin wyjazdu był w piatek po godzinie 19:00,
a potem dorzucić monete 5 zł,
5. Wrzucić 1 zł, oczekiwany termin wyjazdu pół godziny po aktualnym czasie.
6. Wrzucić 200 monet 1gr, oczekiwany termin wyjazdu godzine po aktualnym czasie.
7. Wrzucić 201 monet 1gr, oczekiwana informacja 0 przepełnieniu parkomatu.
8. Wciśnięcie “Zatwierdź” bez wrzucenia monet-- oczekiwana informacja o błędzie.
9. WciSniecie “Zatwierdź” bez wpisania numeru rejestracyjnego -- oczekiwana
informacja o błędzie. Wcisniecie “Zatwierdz” po wpisaniu niepoprawnego
numeru rejestracyjnego -- oczekiwana informacja o błędzie.

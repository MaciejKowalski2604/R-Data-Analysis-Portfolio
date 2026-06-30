# Analiza i dekompozycja szeregów czasowych 📈

Projekt skupia się na diagnostyce szeregów czasowych oraz zaawansowanych metodach dekompozycji i eliminacji trendu. Wykorzystano dane dotyczące miesięcznej sprzedaży leków w Australii (`a10` z pakietu `fpp2`).

## 🛠️ Wykorzystane techniki
- **Weryfikacja białoszumowości:** Testy formalne (Box-Pierce, Ljung-Box) oraz analiza graficzna korelogramów (ACF).
- **Symulacje Monte Carlo:** Badanie empirycznego rozmiaru i mocy testów statystycznych w zależności od długości szeregu, wybranego opóźnienia i typu rozkładu (m.in. Normalny, t-Studenta, MA(1), Błądzenie Losowe).
- **Dekompozycja szeregu:** Transformacja Boxa-Coxa w celu stabilizacji wariancji.
- **Modelowanie trendu i sezonowości:** Porównanie modeli addytywnych, multiplikatywnych, modeli regresji liniowej/kwadratowej (TSLM) oraz zaawansowanej dekompozycji STL.
- **Narzędzia:** R (`forecast`, `fpp2`, `stats`, `ggplot2`).

## 📂 Struktura projektu
- `time_series_analysis.Rmd` - kod źródłowy z analizą i symulacjami.
- `time_series_analysis.pdf` - wyrenderowany raport z wykresami i interpretacją wyników.

## 🚀 Kluczowe wnioski
1. **Test Ljunga-Boxa** wykazuje przewagę nad testem Boxa-Pierce'a, szczególnie w przypadku krótkich szeregów czasowych.
2. Zastosowanie **transformacji Boxa-Coxa** jest kluczowe dla ustabilizowania wariancji przed modelowaniem szeregów o charakterze multiplikatywnym.
3. Metoda **STL** (Seasonal and Trend decomposition using Loess) okazała się najskuteczniejsza w izolowaniu sygnału, minimalizując wariancję reszt lepiej niż sztywne modele TSLM.
# Analiza Przeżycia (Survival Analysis) i Symulacje Monte Carlo ⏳

Projekt koncentruje się na statystycznej analizie przeżycia. Obejmuje symulacje rozkładów, estymację parametrów przy danych cenzurowanych oraz badanie mocy testów statystycznych.

## 🛠️ Wykorzystane techniki i zagadnienia
- **Rozkłady:** Eksponencjalny $E(\vartheta)$ oraz Weibulla (EW), badanie różnych kształtów funkcji hazardu (rosnąca, malejąca, wannowa).
- **Cenzurowanie danych:** Implementacja cenzurowania typu I, typu II oraz cenzurowania losowego.
- **Estymacja:** Wyznaczanie estymatorów Największej Wiarogodności (MLE) dla parametrów intensywności oraz konstruowanie przedziałów ufności (np. metodą Cloppera-Pearsona).
- **Testowanie hipotez:** Asymptotyczny test ilorazu wiarogodności (LRT) oraz symulacje Monte Carlo do weryfikacji rozmiaru i empirycznej mocy testu.
- **Narzędzia:** R (`ggplot2`, `dplyr`, `patchwork`).

## 📂 Struktura projektu
- `survival_analysis.Rmd` - kod źródłowy R implementujący generatory zmiennych losowych, estymatory i symulacje.
- `survival_analysis.pdf` - kompletny raport statystyczny z wykresami (m.in. funkcje gęstości, dystrybuanty empiryczne, testy).

## 🚀 Kluczowe wnioski
1. Zwiększenie liczebności próby znacząco poprawia empiryczną moc testu ilorazu wiarogodności (LRT) w badaniach zjawisk przeżycia.
2. Odpowiednie zarządzanie danymi cenzurowanymi (np. pacjenci, u których remisja nie wystąpiła w zadanym czasie) pozwala na rzetelną estymację średniego czasu trwania zjawiska bez odrzucania cennych informacji.
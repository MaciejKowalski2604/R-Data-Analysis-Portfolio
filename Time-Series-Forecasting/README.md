# Prognozowanie szeregów czasowych (SARIMA, ETS, STL) 📈

Projekt koncentruje się na dopasowywaniu zaawansowanych modeli prognostycznych do rzeczywistych danych (globalne temperatury oraz sprzedaż detaliczna w strefie euro) wraz z kompleksową diagnostyką i oceną dokładności prognoz.

## 🛠️ Wykorzystane techniki
- **Modele prognostyczne:** SARIMA, wygładzanie wykładnicze (ETS), dekompozycja STL.
- **Transformacje:** Różnicowanie, eliminacja trendu deterministycznego, transformacja Boxa-Coxa.
- **Diagnostyka modeli:** Analiza reszt (testy Ljunga-Boxa, Shapiro-Wilka, punktów zwrotnych), weryfikacja istotności parametrów (MLE vs Yule-Walker).
- **Ocena dokładności:** Podział na zbiór uczący i testowy (Train/Test split), ewaluacja prognoz za pomocą metryk RMSE, MAE, MAPE, MASE.
- **Narzędzia:** R (`forecast`, `astsa`, `fpp2`, `ggplot2`).

## 📂 Struktura projektu
- `forecasting_models.Rmd` - kod analizy, budowy modeli i ewaluacji.
- `forecasting_models.pdf` - raport końcowy z wynikami.

## 🚀 Kluczowe wnioski
1. Model ARIMA (z wcześniejszą transformacją Boxa-Coxa) okazał się najskuteczniejszy w prognozowaniu sprzedaży detalicznej w okresie spadku koniunktury, przewyższając metody naiwne i dekompozycyjne.
2. Podział danych na zbiór uczący i testowy potwierdził, że zastosowane modele zachowały zdolność generalizacji (brak zjawiska overfittingu).
3. Różnicowanie szeregu jest bezpieczniejszym podejściem do ustatyczniania stochastycznych danych klimatycznych niż sztywna ekstrapolacja trendu wielomianowego.
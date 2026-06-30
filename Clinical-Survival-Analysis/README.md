# Kliniczna Analiza Przeżycia (Survival Analysis) 🏥

Projekt stanowi praktyczne zastosowanie nieparametrycznych metod analizy przeżycia do oceny skuteczności leków oraz analizy czasu do progresji choroby pacjentek z rakiem jajnika (dane z Mayo Clinic).

*Projekt zrealizowany we współpracy z Mateuszem Wiznerem.*

## 🛠️ Wykorzystane techniki
- **Estymacja funkcji przeżycia $S(t)$:** Estymatory Kaplana-Meiera oraz Fleminga-Harringtona.
- **Radzenie sobie z cenzurowaniem:** Zastosowanie korekty ogona metodą Browna-Hollandera-Kowara (BHK) do szacowania długoterminowego prawdopodobieństwa przeżycia.
- **Średni czas przeżycia:** Obliczanie Restricted Mean Survival Time (RMST) wraz z przedziałami ufności.
- **Weryfikacja hipotez:** Testowanie równości rozkładów za pomocą testów rangowych: Log-rank, Gehan-Breslow, Tarone-Ware oraz Peto-Peto.
- **Narzędzia:** R (`survival`, `survminer`, `ggplot2`, `coin`).

## 📂 Struktura
- `clinical_survival_analysis.Rmd` - kod analityczny w R.
- `clinical_survival_analysis.pdf` - wyrenderowany, pełny raport z wizualizacjami i wnioskami statystycznymi.

## 🚀 Kluczowe wnioski
1. Estymacja średniego czasu do remisji często wymaga zastosowania korekty BHK dla danych cenzurowanych prawostronnie.
2. Dobór odpowiedniego testu statystycznego ma kluczowe znaczenie: test Gehana-Breslowa wykrył istotne różnice we wczesnej fazie leczenia, które zostały zignorowane przez klasyczny test Log-rank ze względu na przecinanie się krzywych przeżycia (brak proporcjonalności hazardów).
# Klasyfikacja i porównanie modeli (Vehicle Dataset) 🚗

Projekt zawiera porównanie skuteczności metod klasyfikacji: OVR (One-vs-Rest) opartej na regresji liniowej, k-NN, CART oraz naiwnego Bayesa.

## 🛠️ Wykorzystane techniki
- **Modele klasyfikacyjne:** 
  - Regresja liniowa OVR (wielomianowa 2. stopnia).
  - k-NN (k-nearest neighbors).
  - CART (Classification and Regression Trees).
  - Naive Bayes.
- **Ocena modeli:** Macierze pomyłek, metryki Accuracy oraz Makro-F1, PCA dla wizualizacji struktury klas.
- **Narzędzia:** R (`caret`, `rpart`, `class`, `e1071`, `ggplot2`).

## 📂 Struktura
- `vehicle_analysis.Rmd` - kompletny kod eksperymentów.
- `vehicle_analysis.pdf` - wyrenderowany raport analityczny.
- `data/` - zbiory danych (zbiór `Vehicle` z pakietu `mlbench`).

## 🚀 Kluczowe wnioski
1. **Regresja liniowa (OVR):** Osiąga wysoką dokładność na zbiorze `Iris`, a dodanie cech wielomianowych poprawia wyniki dla trudniej rozróżnialnych klas.
2. **Porównanie klasyfikatorów:** Model k-NN zapewnia najlepszą równowagę między metrykami, podczas gdy CART jest najbardziej wartościowy dla interpretacji biznesowej.
3. **Wizualizacja:** PCA potwierdza, że niektóre klasy (np. *saab* i *van*) nakładają się w przestrzeni cech, co generuje główne pomyłki modeli.
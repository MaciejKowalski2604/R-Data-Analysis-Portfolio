# Eksploracja danych, PCA i MDS 

Projekt zawiera raport z analizy danych, w którym skupiono się na technikach eksploracyjnych oraz redukcji wymiarowości.

## 🛠️ Wykorzystane techniki
- **Dyskretyzacja:** Porównanie metod (Equal width, Frequency, K-means, tercyle) na zbiorze `iris`.
- **PCA (Principal Component Analysis):** Wykorzystane do redukcji wymiarów zbioru *City Quality of Life* oraz interpretacji ładunków zmiennych.
- **MDS (Multidimensional Scaling):** Zastosowane do wizualizacji struktury zbioru *Titanic* w przestrzeni 2D.
- **Analiza skupień:** Porównanie algorytmów PAM i AGNES przy użyciu wskaźników Silhouette i ARI.

## 📂 Struktura projektu
- `eda_pca_mds.Rmd` - kompletny kod R wraz z analizą.
- `eda_pca_mds.pdf` - wyrenderowany raport w formacie PDF.
- `data/` - pliki z danymi wejściowymi.

## 🚀 Kluczowe wnioski
- Metody klastrowania (PAM, AGNES) pozwalają odkryć naturalną strukturę danych bez wcześniejszej znajomości etykiet.
- W redukcji wymiarów (PCA), standaryzacja cech była kluczowa dla poprawnej interpretacji głównych składowych.
- PCA i MDS stanowią potężne narzędzia do wizualizacji zbiorów wielowymiarowych.
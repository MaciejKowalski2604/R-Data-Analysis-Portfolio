# Analiza Rezygnacji Klientów (Telco Customer Churn EDA) 📊

Projekt obejmuje kompleksową, eksploracyjną analizę danych (EDA) klientów firmy telekomunikacyjnej. Celem analizy jest identyfikacja kluczowych czynników wpływających na decyzję klientów o odejściu (Churn) oraz sformułowanie rekomendacji biznesowych.

## 🛠️ Wykorzystane technologie
- **Język:** R
- **Biblioteki:** `dplyr`, `ggplot2`, `DataExplorer`, `tidyr`
- **Raportowanie:** R Markdown, `knitr`, `kableExtra`

## 📂 Struktura projektu
- `churn_analysis.Rmd` - kod źródłowy analizy, czyszczenie danych i generowanie wykresów.
- `churn_analysis.pdf` - gotowy, wyrenderowany raport analityczny z wnioskami.
- `data/` - zbiór danych pobrany z platformy Kaggle.

## 🚀 Kluczowe wnioski z analizy
Z przeprowadzonych podziałów na kohorty (klienci, którzy odeszli vs pozostali) wynika, że największe ryzyko rezygnacji występuje u klientów, którzy:
1. Posiadają umowy krótkoterminowe (odnawiane z miesiąca na miesiąc).
2. Płacą wyższe abonamenty miesięczne, ale mają bardzo krótki staż (tenure).
3. Nie korzystają z dodatkowych usług zabezpieczających (np. Online Security, Tech Support).
4. Korzystają z połączeń światłowodowych (Fiber optic), co może sugerować niezadowolenie z jakości tej konkretnej usługi u tego dostawcy.
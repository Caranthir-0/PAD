# Analiza urazów serca
Projekt zaliczeniowy PAD - S34686 Konrad Obrebski

---

## Opis projektu
Projekt ma na celu analizę danych dotyczących urazów serca oraz budowę modeli predykcyjnych, które pomagają diagnozować choroby serca na podstawie dostępnych danych. W projekcie przeprowadzono:
- Analizę eksploracyjną (EDA)
- Testowanie hipotez (A/B testing)
- Redukcję wymiarów (PCA)
- Budowę modeli ML (Drzewa Decyzyjne, Regresja Logistyczna, SVC, RandomForestClassifier)

---

## Instrukcja uruchomienia

1. **Wymagane oprogramowanie:**
   - Python 3.8+
   - Wymagane biblioteki: NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, Plotly, Dash, XGBoost

   Zainstaluj wszystkie wymagane biblioteki za pomocą:
   ```bash
   pip install -r requirements.txt
   ```

2. **Uruchomienie projektu:**
   - Otwórz plik `PAD_PROJECT.ipynb` w Jupyter Notebook lub JupyterLab.
   - Wykonaj wszystkie komórki w odpowiedniej kolejności.

3. **Dashboard (jeśli dotyczy):**
   - Wykorzystano bibliotekę Dash oraz Dash Bootstrap Components do stworzenia dashboardu.
   - Aby uruchomić dashboard, użyj:
     ```bash
     python app.py
     ```
     (plik `app.py` powinien znajdować się w folderze projektu).

---

## Struktura projektu

- `PAD_PROJECT.ipynb`: Główny notebook zawierający całą analizę, modelowanie i wizualizacje.
- `data/`: Folder na dane (brak plików danych w notebooku, dane muszą być dostarczone).
- `requirements.txt`: Lista wymaganych bibliotek do uruchomienia projektu.
- `README.md`: Dokumentacja projektu.

---

## Dane
Dane wykorzystane w projekcie:
- **age**: wiek w latach
- **sex**: płeć (1=mężczyzna, 2=kobieta)
- **cp**: typ bólu w klatce piersiowej
- **trestbps**: spoczynkowe ciśnienie krwi
- **chol**: poziom cholesterolu
- ... *(pozostałe zmienne opisane są w notebooku)*

Źródło danych: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/index.php)

---

## Wnioski
- W projekcie przeanalizowano istotne zmienne wpływające na diagnozę chorób serca.
- Najlepszym modelem okazał się RandomForestClassifier z najwyższą dokładnością i zrównoważonym F1 Score.


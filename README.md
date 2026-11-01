# Axion-kolo

Wyzwanie 3: Quantum Machine Learning (QML)

**Hipoteza:**
Zastosowanie najbardziej zasobożennej topologii splątania `full` nie polepszy accuracy na prostym zbiorze danych `make_moons`, w porównaniu do oszczędnej topologii `linear`. Spowoduje za to drastyczne i niepotrzebne wydłużenie czasu treningu.

**Przewidywany wynik:**
Po narysowaniu learning curves spodziewam się, że model z topologią `linear` osiągnie dobre accuracy w podobnej liczbie epok co `full`, ale pojedyńcza epoka będzie dla topologii `full` trwała znacznie dłużej z powodu nadmiaru bramek.

---

**Prediction:**
Przewidywanie sprawdziło się, topologia full nie poprawiła wyników, a wręcz pogorszyła zdolność modelu do nauki.

**Full:**
Zbyt gęste splątanie w obwodzie full doprowadziło do overparameterization, przez co optymalizator szybko utknął z  wyższym błędem końcowym.

**Linear:**
Oszczędna topologia linear jest wystarczająca i optymalna dla prostego zbioru danych make_moons.

**"Co by było, gdyby…":**
Zwiększenie głębokości sprawiłoby, że model 'linear' straciłby swoją przewagę i zacząłby zachowywać się równie źle co model 'full'. Dla tak prostych danych wejściowych optymalizator dostałby zbyt wiele wag do dostosowania, co doprowadziłoby do niestabilności, poszarpanej krzywej uczenia i ryzyka utknięcia w barren plateaus.

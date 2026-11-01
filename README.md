# Axion-kolo

Wyzwanie 3: Quantum Machine Learning (QML)

**Hipoteza:**
Zastosowanie najbardziej zasobożennej topologii splątania `full` nie polepszy accuracy na prostym zbiorze danych `make_moons`, w porównaniu do oszczędnej topologii `linear`. Spowoduje za to drastyczne i niepotrzebne wydłużenie czasu treningu.

**Przewidywany wynik:**
Po narysowaniu learning curves spodziewam się, że model z topologią `linear` osiągnie dobre accuracy w podobnej liczbie epok co `full`, ale pojedyńcza epoka będzie dla topologii `full` trwała znacznie dłużej z powodu nadmiaru bramek.

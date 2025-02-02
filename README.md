Raport z analizy modelu przewidywania depresji wśród studentów

1. Wprowadzenie

Projekt dotyczy analizy depresji wśród studentów na podstawie dostępnych danych. Głównym celem jest stworzenie modelu predykcyjnego, który może pomóc w identyfikacji studentów zagrożonych depresją.

2. Opis przeprowadzonych operacji

2.1 Wczytanie i przygotowanie danych

Zaimportowano dane dotyczące studentów, zawierające cechy demograficzne, akademickie i psychologiczne.

Dokonano analizy brakujących wartości i zastosowano odpowiednie techniki uzupełniania danych (np. imputacja wartości średnich), aby uniknąć utraty istotnych informacji i poprawić jakość modelu.

Przekształcono zmienne kategoryczne na format numeryczny (one-hot encoding, label encoding), co było konieczne do wykorzystania algorytmów uczących się na danych liczbowych.

Dokonano normalizacji wartości numerycznych w celu poprawy jakości modelu i zapewnienia lepszej konwergencji algorytmów.

2.2 Eksploracyjna analiza danych (EDA)

Przeanalizowano rozkłady zmiennych oraz ich korelację z występowaniem depresji, aby zrozumieć wpływ poszczególnych cech na zmienną docelową.

Wykorzystano wykresy (histogramy, wykresy pudełkowe) do wizualizacji danych, co ułatwiło identyfikację potencjalnych zależności i anomalii w zbiorze danych.

Sprawdzono zależności między zmiennymi a zmienną docelową (depresja), co pozwoliło na wybór najbardziej informatywnych cech do budowy modelu.

2.3 Budowa modelu

Podzielono dane na zbiór treningowy i testowy w stosunku 80/20, aby zapewnić odpowiednią generalizację modelu.

Zastosowano różne algorytmy klasyfikacyjne, m.in. regresję logistyczną, drzewa decyzyjne, las losowy oraz SVM, aby wybrać najbardziej skuteczny model.

Dokonano strojenia hiperparametrów przy użyciu walidacji krzyżowej, co pozwoliło na optymalizację modelu i poprawę jego skuteczności.

Wybrano model o najlepszej skuteczności na podstawie metryk jakościowych, aby zapewnić jak najwyższą trafność klasyfikacji przypadków depresji.

2.4 Ewaluacja modelu

Ocena skuteczności modelu na podstawie miar takich jak:

Accuracy (dokładność klasyfikacji) – pozwala określić ogólną skuteczność modelu.

Precision (precyzja wykrywania przypadków depresji) – kluczowa w kontekście minimalizacji fałszywie pozytywnych wyników.

Recall (czułość w wykrywaniu depresji) – istotna dla maksymalizacji liczby poprawnie wykrytych przypadków.

F1-score (harmoniczna średnia precision i recall) – zapewnia zrównoważoną ocenę modelu.

ROC-AUC (obszar pod krzywą ROC) – mierzy zdolność modelu do odróżniania przypadków depresji od tych, którzy jej nie wykazują.

Wykorzystano macierz błędów (confusion matrix) do oceny błędnych klasyfikacji i zrozumienia, gdzie model popełnia najwięcej błędów.

3. Analiza wyników



Najlepszy wynik pod względem F1-score uzyskał model Random Forest, co sugeruje, że jest on najlepszym wyborem do wykrywania depresji wśród studentów.

Wysoka wartość ROC-AUC (91%) sugeruje, że model dobrze odróżnia studentów zagrożonych depresją od tych, którzy nie wykazują jej objawów.

Model może wymagać dalszego strojenia hiperparametrów lub uwzględnienia dodatkowych zmiennych celem poprawy skuteczności.

4. Interpretacja wykresów

Histogramy – Pokazują rozkład zmiennych, np. poziom stresu, czas snu czy oceny akademickie. Pomagają zrozumieć, jakie wartości są najczęstsze i czy dane mają rozkład normalny.

Wykresy pudełkowe (Boxploty) – Ilustrują rozkład zmiennych oraz obecność wartości odstających, np. w zakresie poziomu stresu studentów.

Macierz korelacji (Heatmapa) – Pokazuje zależności między zmiennymi, np. czy stres jest silnie skorelowany z wynikami akademickimi lub poziomem aktywności fizycznej.

Wykres ROC-AUC – Obrazuje skuteczność modelu w rozróżnianiu przypadków depresji i zdrowych studentów. Im większe pole pod krzywą, tym lepszy model.

Macierz błędów (Confusion Matrix) – Prezentuje liczbę poprawnych i błędnych klasyfikacji, co pozwala ocenić, w jakich przypadkach model najczęściej się myli.

5. Wnioski

Opracowany model ma duży potencjał w zakresie przewidywania depresji wśród studentów.

Istnieje możliwość poprawy wyników poprzez zebranie większej ilości danych oraz zastosowanie bardziej zaawansowanych modeli.

Wyniki sugerują, że pewne zmienne mają silniejszy wpływ na depresję, co może być przydatne w badaniach nad zdrowiem psychicznym studentów.

Wysoka częstość występowania depresji wśród studentów podkreśla konieczność wdrażania skutecznych programów wsparcia psychologicznego.

Styl życia, poziom stresu oraz relacje społeczne odgrywają kluczową rolę w występowaniu depresji, co wskazuje na potrzebę holistycznego podejścia do zdrowia psychicznego.

6. Możliwe dalsze kroki

Implementacja modelu w aplikacji wspierającej doradców akademickich.

Dalsza analiza wpływu różnych czynników na depresję studentów.

Rozszerzenie zbioru danych o dodatkowe atrybuty psychologiczne i społeczne.






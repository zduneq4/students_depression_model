Raport z analizy modelu przewidywania depresji wśród studentów
1. Wprowadzenie
Projekt dotyczy analizy depresji wśród studentów na podstawie dostępnych danych. Głównym celem jest stworzenie modelu predykcyjnego, który może pomóc w identyfikacji studentów zagrożonych depresją.
2. Opis przeprowadzonych operacji

2.1 Wczytanie i przygotowanie danych
- Zaimportowano dane dotyczące studentów, zawierające cechy demograficzne, akademickie i psychologiczne.
- Dokonano analizy brakujących wartości i zastosowano odpowiednie techniki uzupełniania danych.
- Przekształcono zmienne kategoryczne na format numeryczny.
- Dokonano normalizacji wartości numerycznych w celu poprawy jakości modelu.

2.2 Eksploracyjna analiza danych (EDA)
- Przeanalizowano rozkłady zmiennych oraz ich korelację z występowaniem depresji.
- Wykorzystano wykresy do wizualizacji danych.
- Sprawdzono zależności między zmiennymi a zmienną docelową.

2.3 Budowa modelu
- Podzielono dane na zbiór treningowy i testowy w stosunku 80/20.
- Zastosowano różne algorytmy klasyfikacyjne.
- Dokonano strojenia hiperparametrów przy użyciu walidacji krzyżowej.
- Wybrano model o najlepszej skuteczności.

2.4 Ewaluacja modelu
- Ocena skuteczności modelu na podstawie accuracy, precision, recall, F1-score i ROC-AUC.
- Wykorzystano macierz błędów do oceny błędnych klasyfikacji.

3. Analiza wyników
- Model uzyskał accuracy na poziomie **87%**, co wskazuje na **dobrą** skuteczność.
- Najlepszy wynik pod względem F1-score uzyskał model **Random Forest**.
- Wysoka wartość ROC-AUC (**91%**) sugeruje, że model dobrze odróżnia studentów zagrożonych depresją.
- Model może wymagać dalszego strojenia hiperparametrów.

4. Wnioski
- Opracowany model ma **duży potencjał** w zakresie przewidywania depresji.
- Istnieje możliwość poprawy wyników poprzez **zebranie większej ilości danych oraz zastosowanie bardziej zaawansowanych modeli**.
- Wyniki sugerują, że pewne zmienne mają silniejszy wpływ na depresję.

5. Możliwe dalsze kroki
- Implementacja modelu w aplikacji wspierającej doradców akademickich.
- Dalsza analiza wpływu różnych czynników na depresję studentów.
- Rozszerzenie zbioru danych o dodatkowe atrybuty psychologiczne i społeczne.

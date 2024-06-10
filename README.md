# Analiza i predykcja chorób serca za pomocą języka Python

&nbsp;
## Opis projektu:

To jest mój pierwszy projekt Data Science, który koncentruje się na analizie i predykcji chorób serca. Głównym celem projektu jest zrozumienie, które czynniki mają największy wpływ na ryzyko wystąpienia zawału serca oraz stworzenie modelu predykcyjnego, który pomoże w identyfikacji osób zagrożonych tą chorobą.

## Cel projektu:

Celem projektu jest analiza danych dotyczących pacjentów z różnymi schorzeniami serca.
Zrozumienie, które czynniki mają największy wpływ na wystąpienie zawału serca.
Stworzenie modelu predykcyjnego, który będzie w stanie dokładnie przewidzieć, czy dany pacjent jest narażony na zawał serca.
Porównanie dwóch modeli klasyfikacyjnych: regresji logistycznej oraz LGBMClassifier, aby wybrać bardziej efektywny model.

## Dane:

Zbiór danych pochodzi z repozytorium UCI Machine Learning i zawiera informacje o pacjentach, takie jak:

- Wiek (age)
- Płeć (sex)
- Rodzaj bólu w klatce piersiowej (chest_pain_type)
- Ciśnienie krwi (resting_bp_s)
- Poziom cholesterolu (cholesterol)
- Poziom cukru we krwi na czczo (fasting_blood_sugar)
- Wyniki elektrokardiograficzne (resting_ecg)
- Maksymalne tętno (max_heart_rate)
- Występowanie duszności wysiłkowej (exercise_angina)
- Wynik testu ST (ST_slope)

## Analiza danych:

Eksploracja danych: Sprawdziłam podstawowe statystyki, wartości brakujące oraz rozkłady zmiennych. Zauważyłam, że dane są względnie zbalansowane.

Wizualizacja danych: Stworzyłam różne wykresy, aby zrozumieć, jak poszczególne zmienne wpływają na wystąpienie zawału serca.
Korelacja: Analiza korelacji pozwoliła zidentyfikować, które zmienne są ze sobą powiązane.

## Wybór cech (feature selection):

Do analizy wybrałam zmienne, które wykazały istotną korelację z celem (target) oraz te, które są istotne z medycznego punktu widzenia. Wybór zmiennych był również oparty na analizie punktów skrajnych i ich wpływu na model.

## Modele:

Regresja logistyczna: Jest to prosty, interpretowalny model, który dobrze radzi sobie z klasyfikacją binarną.
LGBMClassifier: Jest to bardziej zaawansowany model, który często osiąga lepsze wyniki w przypadku większych i bardziej złożonych zbiorów danych.

## Wyniki:

Regresja logistyczna: Uzyskana dokładność na zbiorze testowym to około 86%. Model ten był w stanie dobrze klasyfikować pacjentów, ale miał pewne ograniczenia w precyzji.
LGBMClassifier: Uzyskana dokładność na zbiorze testowym to około 95%. Model ten przewyższał regresję logistyczną zarówno pod względem dokładności, jak i precyzji.

# Wnioski:

Model LGBMClassifier okazał się bardziej efektywny w przewidywaniu ryzyka zawału serca. Jego większa dokładność i precyzja sprawiają, że jest lepszym wyborem do tego zadania. W przyszłości warto zbadać wpływ innych zmiennych oraz zastosować inne metody przetwarzania danych, aby jeszcze bardziej poprawić wyniki modelu.

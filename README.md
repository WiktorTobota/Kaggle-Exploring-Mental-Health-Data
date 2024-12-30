# Rozwiązanie konkursu Kaggle: Exploring-Mental-Health-Data

## Opis projektu
To repozytorium zawiera moje rozwiązanie konkursu organizowanego przez Kaggle. Celem konkursu jest przewidzenie zmiennej `Depression` (wartości binarnej: 0 lub 1).

Dane treningowe i testowe zawierają różne cechy opisujące osoby, takie jak wiek, płeć, wykonywany zawód, liczba godzin pracy/nauki, nawyki żywieniowe, itp. Wyzwanie polega na przygotowaniu danych, zbudowaniu modelu klasyfikacyjnego i zgłoszeniu przewidywanych wartości dla zbioru testowego.

## Zastosowane podejście
1. **Eksploracyjna analiza danych**:
   - Wyświetlenie podstawowych informacji i statystyk opisowych dla danych.
   - Wizualizacja brakujących wartości przy użyciu biblioteki `missingno`.
   - Sortowanie danych w celu analizy grup (np. profesjonalistów i studentów).

2. **Przygotowanie danych**:
   - Uzupełnianie brakujących wartości w kolumnach numerycznych (średnią z kolumny) oraz kategorycznych (na podstawie innych cech).
   - Kodowanie zmiennych kategorycznych za pomocą `one-hot encoding`.
   - Dopasowanie kolumn w zbiorze treningowym i testowym.

3. **Modelowanie**:
   - Wykorzystanie regresji logistycznej (`LogisticRegression`) do klasyfikacji binarnej.
   - Trenowanie modelu na danych treningowych.
4. **Wyniki**:
   - Model osiągnął dokładność treningową wynoszącą 94.02%

6. **Ocena i zgłoszenie**:
   - Obliczenie dokładności modelu na danych treningowych.
   - Generowanie przewidywań dla zbioru testowego i zapisanie ich do pliku `submission.csv`.

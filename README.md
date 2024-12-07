Predykcja Zaburzeń Snu

Celem tego projektu jest analiza danych związanych ze stylem życia i zmiennych medycznych, takich jak wiek, BMI, aktywność fizyczna, czas trwania snu, ciśnienie krwi i inne, w celu przewidzenia występowania zaburzeń snu oraz ich rodzaju.

Zestaw Danych

Projekt wykorzystuje zestaw danych Sleep Health and Lifestyle, który zawiera 374 wiersze i 13 kolumn, obejmując szeroki zakres zmiennych związanych ze snem i nawykami życiowymi.

Główne cechy zestawu danych:

Dane o śnie: Czas trwania, jakość snu i inne czynniki wpływające na jego wzorce.

Styl życia: Poziom aktywności fizycznej, poziom stresu oraz BMI.

Zdrowie sercowo-naczyniowe: Pomiary ciśnienia krwi i tętna.

Zaburzenia snu: Informacje o braku zaburzeń, bezsenności oraz bezdechu sennym.

Wyjaśnienie wartości w kolumnie Sleep Disorder:
  None: Brak zaburzeń snu.
  Insomnia: Problemy z zasypianiem lub utrzymaniem snu.
  Sleep Apnea: Przerwy w oddychaniu podczas snu.

![image](https://github.com/user-attachments/assets/9ecffd2a-86b9-48a1-b867-cb41c3ea84aa)


Eksploracja Danych (EDA)
Analiza danych podzielona została na dwie części:

Zrozumienie danych za pomocą wizualizacji:

Większość osób ma jakość snu powyżej 5, co wskazuje na odpowiednią regenerację.
Zawód oraz BMI mają znaczący wpływ na występowanie zaburzeń snu. Pielęgniarki są szczególnie narażone na bezdech senny, podczas gdy osoby z nadwagą częściej mają zaburzenia snu.
Analiza korelacji między zmiennymi:

Silne zależności wykazano między BMI a występowaniem zaburzeń snu.

Przetwarzanie Danych

Brakujące wartości w kolumnie Sleep Disorder zostały uzupełnione jako None.
Zmienne kategoryczne, takie jak płeć czy zawód, zakodowano za pomocą Label Encoding.
Ciśnienie krwi rozdzielono na skurczowe i rozkurczowe, aby ułatwić dalszą analizę.

Budowa Modelu

W projekcie wykorzystano dwa algorytmy klasyfikacyjne do przewidywania zaburzeń snu:

1. Decision Tree Classifier
Dokładność modelu: 86,7%
Wyniki: Model osiągnął dobrą skuteczność, jednak wykazywał pewne rozbieżności w przewidywaniu wartości rzeczywistych.
2. Random Forest Classifier
Dokładność modelu: 89,3%
Wyniki: Model losowego lasu przewyższył klasyfikator drzewa decyzyjnego, osiągając lepsze wyniki w zakresie precyzji i ogólnej dokładności.

Wnioski
Model Random Forest jest bardziej niezawodny w przewidywaniu zaburzeń snu w oparciu o dostępne dane.
Czynniki takie jak zawód, BMI oraz jakość snu są kluczowe w określaniu prawdopodobieństwa wystąpienia zaburzeń snu.

Instrukcja Użycia

1. Upewnij się, że masz zainstalowane niezbędne biblioteki: pandas, numpy, seaborn, matplotlib, sklearn.
2. Wczytaj zestaw danych (Sleep_health_and_lifestyle_dataset.csv) i wykonaj wstępne przetwarzanie danych zgodnie z przedstawionym kodem.
3. Wytrenuj modele (Decision Tree oraz Random Forest) i przeprowadź ich ewaluację.
4. Eksperymentuj z parametrami modeli, aby poprawić ich skuteczność.

Autor:
Projekt stworzony jako przykład wykorzystania technik uczenia maszynowego do analizy danych medycznych i stylu życia.

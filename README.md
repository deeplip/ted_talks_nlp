# Ted Talks NLP
_Klasyfikacja wieloetykietowa (ang. multilabel classification) transkrypcji wystąpień TED ze względu na ich tematykę.
Zbiór danych: kaggle.com_

1. Ograniczenie ilości tematów (kategorii)
    Początkowo różnych tematów wystąpień było 457, co sprawiało, że niektóre kategorie miały bardzo
    małe reprezentacje ilościowe. Na podstawie ilości wystąpień (>400) wybrałem 11 różnych kategorii.
2. Oczyszczanie i przygotowanie danych
    Kodowanie kategoryczne (one-hot), tokenizacja i rdzeniowanie metodami _Snowball_ i _Porter_,
    oczyszczanie ze zbędnych znaków, redukcja rzadkich wyrazów, podział zbioru, wektoryzacja TFIDF
3. Klasyfikacja z użyciem Scikit-multilearn
    Chain classifier, LabelPowerset, BinaryRelevance
4. Klasyfikacja z użyciek Tensorflow.Keras
    Conv1D sequential, Conv1D sequential z uwzględnieniem wagi klas, Conv1D functional 3-wejściowy. 
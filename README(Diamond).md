# Diamond Price Prediction

Bu layihədə diamond xüsusiyyətlərinə əsasən qiymət proqnozu üçün maşın öyrənməsi modeli qurulmuşdur.

## Dataset sütunları
- carat
- cut
- color
- clarity
- depth
- table
- x, y, z ölçüləri
- price (target)

## Görülən işlər
- Data preprocessing
- Kategorik dəyişənlərin encoding edilməsi
- Train/Test bölünməsi
- Boosting regression modelinin qurulması
- Modelin qiymətləndirilməsi

## Nəticə
Model test datada təxminən **R2 ≈ 0.98** nəticə göstərmişdir.

## İstifadə olunan alətlər
Python, Pandas, Scikit-learn

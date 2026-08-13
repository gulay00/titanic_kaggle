# Titanic - Kaggle Layihəsi

Bu, Kaggle-ın Titanic yarışması üçün etdiyim ilk ML layihəmdir. Sərnişinlərin məlumatlarına baxıb kimin sağ qalacağını proqnozlaşdırdım.

Nəticə: leaderboard-da 2757/10951, ~78% accuracy. Model olaraq Random Forest istifadə etdim, GridSearchCV ilə parametrləri tənzimlədim.

## Nə etdim
Əvvəlcə datanı təmizlədim — boş yerləri doldurdum, lazımsız sütunları (Cabin, Name, Ticket) sildim. SibSp və Parch-dan FamilySize adında yeni bir sütun yaratdım. Sex və Embarked kimi mətn sütunlarını rəqəmə çevirdim, sonra hər şeyi scale etdim.

Bir neçə model sınadım — Logistic Regression, Random Forest, Gradient Boosting, XGBoost, SVM, KNN. Ən yaxşı nəticəni Random Forest verdi, ona görə onu seçdim.

## Fayllar
- `titanic_analysis.ipynb` — bütün kod
- `submission.csv` — Kaggle-a göndərdiyim fayl

## İstifadə etdiyim alətlər
Python, Pandas, Scikit-learn, Matplotlib, Seaborn

# 🏀 NBA Player Performance - Anomaly Detection

Acest repository conține un proiect de Machine Learning dedicat detectării anomaliilor (Anomaly Detection) în performanțele jucătorilor din NBA. Utilizând framework-ul **PyOD**, proiectul identifică automat jucătorii cu performanțe atipice – fie superstaruri cu statistici excepționale, fie jucători cu profiluri de joc unice.

## 🎯 Obiectivul Proiectului
Scopul principal este identificarea **anomaliilor globale (Point Anomalies)** în datele de performanță sportivă. În acest context, anomaliile nu reprezintă erori tehnice în date, ci performanțe umane excepționale care deviază semnificativ de la media întregului set de date.

## 🧠 Algoritmi și Modele Utilizate
Sistemul implementează și compară trei metode distincte de detectare a anomaliilor:
* **K-Nearest Neighbors (KNN)**: Modelul a fost optimizat prin analiza de sensibilitate (Elbow Method) pentru a găsi numărul ideal de vecini (k), asigurând stabilitatea și evitând clasificarea zgomotului drept anomalie.
* **Angle-Based Outlier Detection (ABOD)**: Utilizat pentru a analiza varianța unghiurilor dintre punctele de date.
* **Isolation Forest (IForest)**: Un algoritm bazat pe arbori, foarte eficient pentru izolarea rapidă a datelor atipice.

## 📈 Rezultate Cheie
* **Consistență**: A existat un consens puternic între cele trei metode (KNN, ABOD, IForest), toate identificând un nucleu comun de jucători de elită (ex: Nikola Jokic, Giannis Antetokounmpo, Luka Doncic).
* **Validare**: Faptul că anomaliile detectate algoritmic corespund exact cu superstarurile recunoscute în realitate validează capacitatea modelului de a funcționa corect, pur matematic, fără etichete preexistente.
* **Aplicabilitate**: Proiectul demonstrează cum tehnicile de Anomaly Detection pot fi folosite ca un instrument automatizat de **scouting** în sport, evidențiind jucători care ar putea fi trecuți cu vederea într-o analiză manuală.

## 💻 Tehnologii Utilizate
* Python
* Google Colab
* **PyOD** (Python Outlier Detection)
* Scikit-learn
* Pandas, NumPy, Matplotlib

## 🚀 Cum să rulezi proiectul în Google Colab

Acest proiect a fost dezvoltat și este recomandat să fie rulat direct în mediul Google Colab.

1. Descarcă fișierul .ipynb și setul de date (fișierul CSV) din acest repository.
2. Accesează [Google Colab](https://colab.research.google.com/).
3. Alege opțiunea **Upload** din meniul principal și încarcă fișierul `tema2TIA.ipynb`.
4. **Încărcarea setului de date:** Pentru ca notebook-ul să funcționeze, trebuie să încarci manual setul de date. Deschide panoul din partea stângă a ecranului (făcând click pe pictograma în formă de folder/fișier) și trage fișierul CSV cu datele NBA acolo.
5. Pentru a asigura instalarea bibliotecii necesare în mediul Colab, rulează următoarea comandă într-o celulă de cod la începutul notebook-ului:

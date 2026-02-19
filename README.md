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
* Jupyter Notebook
* **PyOD** (Python Outlier Detection)
* Scikit-learn
* Pandas, NumPy, Matplotlib

## 🚀 Cum să rulezi proiectul local

1. Clonează acest repository:
   ```bash
   git clone [https://github.com/username/numele-repository-ului.git](https://github.com/username/numele-repository-ului.git)

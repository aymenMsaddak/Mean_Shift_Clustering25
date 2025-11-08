# Mean Shift Clustering: Theory, Implementation & Crime Hotspot Detection in Sfax

---

## 📑 Table of Contents
- [Overview](#-overview)
- [Key Objectives](#-key-objectives)
- [Project Structure](#-project-structure)
- [Technologies Used](#-technologies-used)
- [How to Run](#-how-to-run)
- [Case Study](#-case-study-crime-hotspots-in-sfax)
- [Results Summary](#-results-summary)
- [References](#-references)
- [Author](#-author)

---

## 📘 Overview
This project explores **Mean Shift Clustering**, a non-parametric, density-based clustering algorithm.  
It combines both **theoretical understanding** and **practical application** through an implementation in Python, using a synthetic **geospatial crime dataset** for Sfax, Tunisia.

The project demonstrates how Mean Shift can automatically identify high-density regions (crime hotspots) without predefining the number of clusters — addressing one of the key limitations of K-Means.

---

## 🧠 Key Objectives
- Understand the **philosophy and motivation** behind Mean Shift.
- Implement Mean Shift Clustering using **scikit-learn**.
- Compare its performance and limitations with **K-Means**.
- Apply the algorithm to a **realistic geospatial case study** (Sfax).
- Visualize clustering results using **Folium interactive maps**.

---

## 🧩 Project Structure
MACHINE LEARNING PROJECT 2025/
│
├── images/
│ Folder containing visual assets or exported figures used in the presentation or notebook.
│
├── IT_430_Mean_Shift_Clustering.pdf
│ Final presentation slides (Beamer LaTeX export).
│
├── mean_shift_clustering.ipynb
│ Main Jupyter Notebook explaining the Mean Shift algorithm, research questions, and experimental results.
│
├── README.md
│ Project documentation (you’re reading it!).
│
├── sfax_crime_data.csv
│ Synthetic dataset containing latitude and longitude points for crime events in Sfax.
│
├── synthetic_sfax_crime_hotspots.ipynb
│ Final notebook generating realistic crime cluster simulation and visualization for Sfax.
│
├── sfax_crime_hotspots.html
│ Interactive Folium map visualizing Mean Shift–detected crime clusters in Sfax.
│
├── sfax_crime_hotspots_heatmap.html
│ Folium heatmap version showing density intensity of crime events in Sfax.
│
├── synthetic_tunis_crime_hotspots.ipynb
│ Jupyter Notebook that generates and clusters synthetic crime data for Tunis (earlier prototype).
│
└── tunisia_synthetic_crime_mean_shift_map.html
Interactive national-level synthetic map of crime clustering using Mean Shift.

---

## 🐍 Technologies Used
- **Python 3.13**
- **NumPy** – numerical computations  
- **pandas** – data handling  
- **scikit-learn** – Mean Shift clustering implementation  
- **Folium** – interactive map visualization  
- **Matplotlib / Seaborn** – optional plots for analysis

---

## 🚀 How to Run

1. **Clone this repository**
   ```bash
   git clone https://github.com/aymenMsaddak/Mean_Shift_Clustering25.git
   cd mean-shift-sfax
2. **Install dependencies**
   pip install numpy pandas scikit-learn folium matplotlib seaborn jupyter
3. **Run the notebook**
   jupyter notebook mean_shift_sfax.ipynb
4. **View the map**
   After execution, open sfax_crime_hotspots.html in your browser.

---

# 🌍 Case Study: Crime Hotspots in Sfax

A synthetic dataset was generated to mimic spatial crime distribution across several neighborhoods:
- Sfax Medina
- Sakiet Ezzit
- Thyna
- El Ain
Additional random noise was added to simulate scattered incidents.
The **Mean Shift** algorithm detected key crime density peaks, plotted interactively on a Folium map.

---

## 📊 Results Summary
- Automatically discovered optimal number of clusters  
- Clearly identified dense crime zones in Sfax  
- Robust to outliers and scattered noise  
- Computationally expensive (`O(n²)`) but effective for medium datasets  

---

## 📚 References
- Comaniciu, D., & Meer, P. (2002). *Mean shift: A robust approach toward feature space analysis*. IEEE TPAMI.  
- Fukunaga, K., & Hostetler, L. (1975). *The estimation of the gradient of a density function*. IEEE Transactions on Information Theory.  
- Silverman, B. W. (1986). *Density Estimation for Statistics and Data Analysis*. Chapman & Hall.  
- Scikit-learn Documentation: [Mean Shift](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.MeanShift.html)  

---

## 🧑‍💻 Author
**Aymen MSADDAK**  
Tunis Business School — Machine Learning Course (Fall 2025)  
Project supervised by Prof. [Montassar BEN MESSAOUD]

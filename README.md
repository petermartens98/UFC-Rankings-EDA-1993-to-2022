# UFC Rankings Data Analysis 🥊📊

This project analyzes historical UFC fighter rankings to uncover trends, longevity, and championship dominance across weight classes. Visualizations such as heatmaps and career ranking trajectories make it easy to understand fighter performance over time.

---

## Table of Contents 📖

1. [Project Overview](##project-overview)
2. [Modules Used](##modules-used)
3. [Data Description](##data-description)
4. [Analysis](##analysis--visualizations)
5. [Visualizations Placeholders](##visualizations-placeholders)
6. [How to Run](##how-to-run)

---

## Project Overview 🎯

The goal of this project is to:

* Analyze UFC fighter rankings historically.
* Identify fighters who spent the most weeks in the rankings.
* Determine the longest reigning champions overall and by weight class.
* Visualize ranking trends over time.

Data is sourced from Kaggle: [UFC Rankings History](https://www.kaggle.com/martj42/ufc-rankings).

---

## Modules Used 🛠️

The following Python modules are utilized in this project:

| Module              | Purpose                                                                             |
| ------------------- | ----------------------------------------------------------------------------------- |
| `pandas`            | Efficient data manipulation, reading CSVs, filtering, and aggregations.             |
| `numpy`             | Numerical operations and handling arrays for calculations and plotting.             |
| `matplotlib.pyplot` | Plotting line charts, customizing axes, titles, and labels.                         |
| `matplotlib.dates`  | Handling and formatting date data in plots.                                         |
| `seaborn`           | Creating visually appealing heatmaps to compare rankings and championship duration. |
| `math`              | Mathematical operations where needed for calculations.                              |
| `os`                | Handling file paths if working with local data.                                     |

> `%matplotlib inline` is used for Jupyter notebooks to display plots directly within the notebook.

---

## Data Description 📂

The dataset (`UFC_rankings_history.csv`) contains:

| Column        | Description                                                      |
| ------------- | ---------------------------------------------------------------- |
| `date`        | Date of the ranking update (YYYY-MM-DD).                         |
| `weightclass` | Weight class of the fighter (e.g., Lightweight, Featherweight).  |
| `fighter`     | Name of the fighter.                                             |
| `rank`        | Ranking of the fighter. Rank `0` indicates the current champion. |

Data Cleaning Steps:

* Converted `date` column to `datetime`.
* Removed any null values.
* Verified data types and counts.

Sample data:

| date       | weightclass     | fighter           | rank |
| ---------- | --------------- | ----------------- | ---- |
| 2013-02-04 | Pound-for-Pound | Anderson Silva    | 1    |
| 2013-02-04 | Pound-for-Pound | Jon Jones         | 2    |
| 2013-02-04 | Pound-for-Pound | Georges St-Pierre | 3    |

---

## Analysis & Visualizations 📊🖼️

### Fighters Ranked the Longest ⏳ & Heatmaps 🔥
* Calculated total weeks each fighter spent in the UFC rankings.
* Top fighters: **Amanda Nunes, Stipe Miocic, Daniel Cormier, José Aldo, Conor McGregor**.
* Heatmaps visualize the **top 20 fighters** by weeks ranked, with color intensity reflecting duration.
<img width="545" height="703" alt="image" src="https://github.com/user-attachments/assets/dd4deede-94cf-4b30-8237-44d73e7d442e" />


### Weight Class Analysis 🏋️‍♂️

* Identified top fighters in each weight class based on weeks ranked.
* Heatmaps provide a visual comparison of fighter consistency across classes.
<img width="532" height="478" alt="image" src="https://github.com/user-attachments/assets/cc061b31-6d53-4233-a9c3-6add97901a3e" />


### Champions Analysis 👑

* Filtered for `rank == 0` to focus on champions.
* Determined longest reigning champions overall and by weight class.
* Top champions: **Amanda Nunes, Demetrious Johnson, Daniel Cormier, Jon Jones, Stipe Miocic**.
* Heatmaps display champion longevity by weight class.
<img width="627" height="793" alt="image" src="https://github.com/user-attachments/assets/8adf9d1b-fe4c-4bb2-bafd-90bb42c46cb1" />
<img width="460" height="470" alt="image" src="https://github.com/user-attachments/assets/2b771d33-1627-4c56-b43b-387582196e24" />

### Rankings Throughout Career 📈

* Plotted rank trajectories for top fighters over time.
* Visualized rises and falls in rankings throughout their UFC careers.
* Y-axis inverted for intuitive ranking visualization (1 = best).
<img width="823" height="1045" alt="image" src="https://github.com/user-attachments/assets/4c013950-8f54-4d21-abf2-7e1ec9eb4fb6" />

---

## How to Run 🏃‍♂️

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/UFC-Rankings-Analysis.git
   ```
2. Install dependencies:

   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Place the CSV file (`UFC_rankings_history.csv`) in the working directory.
4. Open the Jupyter Notebook and run all cells to generate visualizations.

---

## License 📜

This project is open-source under the MIT License.

---

If you want, I can **also make a version with even more playful emojis and visual hierarchy for each section** to make it very GitHub-friendly and visually appealing.

Do you want me to do that?

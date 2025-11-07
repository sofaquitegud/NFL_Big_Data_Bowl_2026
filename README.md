# NFL Big Data Bowl 2026 – Analytics Track

## Overview

This project explores player-tracking data from the **NFL Big Data Bowl 2026 – Analytics competition**. The goal is to understand player behavior and game dynamics through **exploratory data analysis (EDA)** rather than predictive modeling.

The analysis combines 18 weeks of input and output files into a single dataset to study player movement, speed distributions, and positional relationships. Using **Python (Pandas, NumPy, Matplotlib)**, the notebook investigates how attributes such as **speed, acceleration, and distance to the ball** relate to play outcomes.

---

## Objectives

* Load, combine, and clean weekly player-tracking datasets
* Engineer new features (*distance_to_ball_land*, *distance_covered*)
* Explore positional movement and speed characteristics
* Visualize spatial and statistical patterns across player roles

---

## Data Description

The combined dataset contains **560,426 entries** and **25 columns**, including:

* Game and play identifiers
* Player attributes (position, role, side)
* Tracking data (x, y, speed, acceleration, direction, orientation)
* Ball landing coordinates

No missing values were found in the dataset.

---

## Key Findings

* **Wide Receivers (WR)** reached the highest speeds and showed the widest range of movement.
* **Linebackers** and **Defensive Ends** maintained lower, tighter speed ranges.
* Most players stayed within **10–20 yards** of the ball landing point, showing tight clustering around play zones.
* Faster players covered more ground, showing a strong link between **average speed** and **distance covered**.
* **Player weight** was slightly negatively correlated with speed and acceleration.
* Spatial visualizations revealed consistent pursuit and coverage structures across plays.

---

## Visualizations

The notebook includes:

* Speed and acceleration distributions by position
* Distance-to-ball and distance-covered distributions
* Correlation heatmaps between performance variables
* Scatter plots of speed versus distance covered
* Player trajectory visualizations

---

## Tools and Libraries

* **Python**: Pandas, NumPy, Matplotlib
* **Jupyter Notebook** for exploration and visualization

---

## How to Run

1. **Clone or download** this repository:

   ```bash
   git clone https://github.com/<your-username>/nfl-big-data-bowl-2026.git
   cd nfl-big-data-bowl-2026
   ```

2. **Install dependencies**:

   ```bash
   pip install pandas numpy matplotlib jupyter
   ```

3. **Prepare the data**:

   * Place all weekly input and output CSV files in a `data/` directory.
   * Ensure the folder structure matches the expected file paths in the notebook.

4. **Open and run the notebook**:

   ```bash
   jupyter notebook nfl-big-data-bowl-2026-analytics-comp-syafiq.ipynb
   ```

5. **Explore the results**:
   The notebook will generate visualizations and descriptive statistics summarizing player movement, speed, and game structure.

---

## Future Work

* Expand the analysis to include **temporal features**, such as player acceleration over time or reaction speed after ball snap.
* Apply **clustering techniques** to group players by movement patterns or tactical roles.
* Investigate **team-level strategies** using aggregated player data.
* Explore **predictive modeling** to estimate play outcomes based on initial positioning and motion variables.
* Integrate **field position heatmaps** to visualize space control and formation tendencies.

---

## Conclusion

This project translates raw NFL tracking data into measurable insights about player performance and spatial structure. It shows how exploratory analysis can uncover the rhythm, structure, and tactical behavior embedded in high-resolution sports data.

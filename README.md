# Football xG (Expected Goals) Predictive Model ⚽📊

A predictive analytics script written in Python that calculates and visualizes the Expected Goals (xG) metric for football shots. The model evaluates how shot distance, shot angle, and player skill levels dynamically affect the mathematical probability of scoring a goal.

## 🔗 Live Implementation & Concepts
This project demonstrates practical experience in **Data Science foundations**, **Mathematical Modeling (Logistic Regression curves)**, and **Data Visualization**.

---

## 🚀 Product Logic & Formulas
The script simulates two player profiles (`Professional` vs. `Amateur`) and analyzes shot quality using mathematical equations:
* **Distance Evaluation:** Uses a sigmoid logistic function to model how scoring probability decays as distance from the goal increases.
* **Angle Evaluation:** Converts shot angles from degrees to radians and applies a sine transformation to calculate the goalkeeper's exposure.
* **Skill Weighting:** Adjusts weights within the exponential functions to demonstrate how elite players sustain higher scoring probabilities under pressure.
* **Final xG Calculation:** Computes the combined probability: 
  $$\text{xG} = P(\text{Distance}) \times P(\text{Angle})$$

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python 3.x
* **Mathematical Operations:** `NumPy` (Vectorized matrix operations, trigonometric transforms)
* **Data Structuring:** `Pandas`
* **Data Visualization:** `Matplotlib` (Custom probability curve rendering)

---

## 🧪 QA & Analytical Verification Applied
From a Quality Assurance perspective, the script was verified using explicit boundary value and execution checks:
1. **Mathematical Invariant Validation:** Confirmed that output probabilities strictly remain within the valid $[0.0, 1.0]$ boundary, regardless of extreme input values (e.g., $0^\circ$ angles).
2. **Precision & Rounding Controls:** Implemented matrix rounding (`np.round`) to format loose floating-point noise into clean, interpretable analytical outputs.
3. **Data Vectorization Check:** Inspected array shape alignment to guarantee that concurrent calculations across distance and angle arrays do not trigger out-of-bounds execution errors.

---

## ⚙️ How to Run Locally
1. Ensure you have Python and the required libraries installed:
   ```bash pip install numpy pandas matplotlib notebook ```
2. Clone the repository:
```git clone [https://github.com/maciekslomka/xg-predictive-model.git](https://github.com/maciekslomka/xg-predictive-model.git)```
3. Open the Jupyter Notebook:
```jupyter notebook```
(and run the ```xg_analysis.ipynb``` file (or your exact notebook filename).

# ⚽ FIFA 2019 Player Data Analysis

Exploratory Data Analysis (EDA) of the FIFA 2019 player dataset, built with **pandas**, **NumPy**, **Matplotlib**, and **Seaborn** in a Jupyter Notebook.

The project cleans raw player data (e.g. converting market value strings like `€105M` into numeric values), then explores player positions, age distribution, preferred foot, market value, international reputation, and the relationship between a player's current ability ("Overall") and future potential.

## 📊 Key Analyses & Visualizations

- **Position distribution** — how many players play in each position (ST, GK, CB, etc.)
- **Age distribution** — histogram and KDE plot of player ages
- **Preferred foot** — count, share (pie chart), and average market value by preferred foot
- **Position × preferred foot** — player counts and average value across positions, split by foot
- **International reputation vs. potential** — violin, strip, and box plots
- **Overall rating vs. potential** — line plots, overall and split by preferred foot
- **Summary dashboard** — a 2×2 grid combining four of the key plots above

All plots are generated inline when you run the notebook — open it in Jupyter to see them rendered.

## 🛠️ Tech Stack

- Python 3
- Jupyter Notebook
- pandas, NumPy
- Matplotlib, Seaborn

## 📁 Project Structure

```
.
├── Fifa_2019_players_analysis.ipynb   # Main analysis notebook
├── requirements.txt                   # Python dependencies
└── README.md
```

## 📦 Dataset

This project uses the **FIFA 19 complete player dataset** (commonly found on Kaggle, e.g. "FIFA 19 complete player dataset" by karangadiya). The raw CSV file is **not included** in this repository.

To run the notebook yourself:

1. Download the dataset (`Fifa 2019.csv` or similarly named file) from Kaggle.
2. Place it somewhere on your machine (e.g. a local `data/` folder).
3. Open the notebook and update the file path in the data-loading cell:

   ```python
   df = pd.read_csv("path/to/your/Fifa 2019.csv")
   ```

   > Note: the original notebook uses a hardcoded local Windows path — remember to change this to match your own environment.

## ▶️ How to Run

```bash
# Clone the repository
git clone https://github.com/sadiqaliyevv/Fifa-2019-players-analysis
cd <Fifa-2019-players-analysis>

# (Optional) create a virtual environment
python -m venv venv
source venv/bin/activate    # on Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook Fifa_2019_players_analysis.ipynb
```

## 📝 Notes

- This notebook was built as a guided EDA exercise (cell prompts are in Azerbaijani), with all code and visualizations in Python.
- Feel free to fork this project and extend it — e.g. adding correlation heatmaps, top-N player rankings, or a club-level comparison.

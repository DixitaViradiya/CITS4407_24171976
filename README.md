# CITS4407_24171976
Board Games or Bored Games: which type and mechanics of board-game rules
Board Game Geek Dataset Analysis
**Author:** Dixita Viradiya  
**Student ID:** 24171976  

This project contains three Bash scripts to process and analyze a dataset of board games from Board Game Geek.

---

## 📁 Files

### ✅ `empty_cells`
Counts the number of missing (empty) cells in each column of a dataset.

**Usage:**
```bash
./empty_cells bgg_dataset.txt ';'
```

**Output:**
Each column name with the number of empty cells.


### ✅ `Preprocess`
Cleans the raw dataset by:

Converting semicolon separators to tabs
Removing Windows line endings and non-ASCII characters
Replacing decimal commas with dots
Filling in missing IDs
Padding rows to 14 columns


**Usage:**
```bash
./preprocess bgg_dataset.txt > bgg_cleaned.tsv
```

**Output:**
Cleaned dataset saved as bgg_cleaned.tsv.


### ✅ `Analysis`
Analyzes the cleaned data to:

Find the most common game mechanic
Find the most common game domain
Compute correlation between:
Year Published and Rating Average
Complexity and Rating Average


**Usage:**
```bash
./analysis bgg_cleaned.tsv
```

**Output:**
4 lines with the most frequent values and correlation scores.

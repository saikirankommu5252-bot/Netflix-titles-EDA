# 🎬 Netflix Titles – Exploratory Data Analysis

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on a Netflix titles dataset using Python.

The analysis explores the content available on Netflix, including **Movies and TV Shows**, their countries of production, release years, ratings, duration, genres, and other attributes.

The goal is to understand the structure of the dataset, identify missing values, analyze content distribution, and extract meaningful insights from the data.

---

## 📊 Dataset

The dataset contains **8,807 records and 12 columns**.

### Main Columns

* `show_id` – Unique identifier for each title
* `type` – Movie or TV Show
* `title` – Title of the content
* `director` – Director of the content
* `cast` – Cast members
* `country` – Country of production
* `date_added` – Date the title was added to Netflix
* `release_year` – Original release year
* `rating` – Content rating
* `duration` – Movie duration or number of seasons
* `listed_in` – Genre/category
* `description` – Description of the title

---

## 🛠️ Technologies Used

* Python
* Jupyter Notebook
* Pandas
* Matplotlib
* Seaborn

---

## 🔍 EDA Process

The following steps were performed in this project:

### 1. Data Loading

The dataset was loaded using Pandas:

```python
df = pd.read_csv("netflix.csv")
```

### 2. Data Understanding

Checked:

* Dataset shape
* Column data types
* Initial records
* Dataset structure

The dataset contains **8,807 rows and 12 columns**.

### 3. Missing Value Analysis

Missing values were analyzed using:

```python
df.isnull().sum()
```

Significant missing values were found in:

* `director` – 2,634
* `cast` – 825
* `country` – 831
* `date_added` – 10
* `rating` – 4
* `duration` – 3

### 4. Duplicate Value Analysis

Duplicate records were checked using:

```python
df.duplicated().sum()
```

The dataset contains **no duplicate rows**.

### 5. Movie vs TV Show Analysis

The distribution of content types was analyzed.

| Type    | Count |
| ------- | ----: |
| Movie   | 6,131 |
| TV Show | 2,676 |

Movies make up a larger portion of the Netflix dataset than TV Shows.

### 6. Country Analysis

The top countries by number of titles were analyzed.

The United States has the highest number of titles, followed by India and the United Kingdom.

### 7. Release Year Analysis

The number of titles released in different years was explored to understand Netflix's content distribution over time.

---

## 💡 Key Insights

* Netflix contains significantly more **Movies than TV Shows** in this dataset.
* There are **6,131 Movies** and **2,676 TV Shows**.
* The **United States** contributes the largest number of titles.
* **India** is the second-highest contributor among the countries shown in the analysis.
* The dataset contains several missing values, particularly in the `director`, `cast`, and `country` columns.
* No duplicate records were found in the dataset.
* Netflix content increased substantially in the later years of the analyzed release-year range.

---

## 📈 Visualizations

The Jupyter Notebook contains visualizations created using **Matplotlib and Seaborn** to understand:

* Movie vs TV Show distribution
* Country-wise content distribution
* Release-year trends
* Other patterns in the Netflix dataset

---

## 📁 Project Structure

```text
netflix-titles-eda/
│
├── netflix.ipynb
├── netflix.csv
└── README.md
```

---

## 🚀 How to Run

1. Clone this repository:

```bash
git clone https://github.com/saikirankommu5252-bot/Netflix-titles-EDA.git
```

2. Open the project folder.

3. Install the required libraries:

```bash
pip install pandas matplotlib seaborn jupyter
```

4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `netflix.ipynb` and run the cells.

---

## 🎯 Conclusion

This project demonstrates the use of **Python, Pandas, Matplotlib, and Seaborn** for performing Exploratory Data Analysis.

The analysis provides an overview of Netflix's content library and highlights patterns related to content type, country, release year, and missing data.

---

## 👨‍💻 Author

**Saikiran Kommu**

GitHub: `https://github.com/saikirankommu5252-bot`

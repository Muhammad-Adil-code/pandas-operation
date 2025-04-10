
# 🎬 IMDb Movie Dataset - NumPy Operations 📊

This project demonstrates **NumPy operations** on a real-world IMDb movie dataset. You'll explore array manipulations, mathematical functions, and data analysis techniques essential for beginners in **Python Data Science**.

---

## 🧠 Dataset Overview

The dataset contains various attributes of movies like:

- 🎬 `Movie_Title`
- 📅 `Year`
- 🧑‍🎤 `Actors`
- 🌟 `Rating`
- 🕐 `Runtime(Mins)`
- 💰 `Total_Gross`

We mainly focus on **numerical columns** (like `Rating`, `Runtime`) for performing NumPy operations.

---

## 📊 Common NumPy Functions – Reference Table

| 🔧 Function       | 💡 Purpose                                     |
|------------------|-----------------------------------------------|
| `.shape`         | Know the structure of the data (rows, columns) |
| `.size`          | Total number of elements in the array          |
| `.ndim`          | Number of dimensions (1D, 2D, etc.)            |
| `.dtype`         | Type of data (e.g., int, float, object)        |
| `np.max()`       | Find the **maximum value**                     |
| `np.min()`       | Find the **minimum value**                     |
| `np.argmax()`    | Get **index of the maximum** value             |
| `np.argmin()`    | Get **index of the minimum** value             |

---

## 🧪 NumPy Operations

### 1️⃣ Copying Arrays 📝

```python
ratings_copy = ratings.copy()
```

- Creates a **backup copy** of an array to avoid modifying the original.

---

### 2️⃣ Append & Insert ➕📍

```python
ratings_appended = np.append(ratings, 9.5)
ratings_inserted = np.insert(ratings, 0, 8.0)
```

- `append()` adds an item at the **end**.
- `insert()` adds at a **specific index**.

---

### 3️⃣ Sorting 🧮

```python
ratings_sorted = np.sort(ratings)
```

- Sorts array in **ascending order**.

---

### 4️⃣ Deleting Elements ❌

```python
ratings_deleted = np.delete(ratings, 0)
```

- Deletes element at index `0`.

---

### 5️⃣ Combining / Concatenation 🔗

```python
combined = np.concatenate((ratings, runtime))
```

- Merges arrays into one.

---

### 6️⃣ Splitting Arrays ✂️

```python
split_data = np.array_split(ratings, 3)
```

- Splits an array into equal parts.

---

### 7️⃣ Indexing & Logical Selection 🔍

```python
high_ratings = ratings[ratings > 8.5]
```

- Returns elements **greater than 8.5**.

---

### 8️⃣ Broadcasting 🧠

```python
ratings_plus_one = ratings + 1
```

- Applies operation to **all elements** in the array at once.

---

### 9️⃣ Type Casting 🔁

```python
ratings_int = ratings.astype(int)
```

- Converts float to **integer values**.

---

### 🔟 Arithmetic Operations ➕➖✖️➗

```python
add = ratings + 1
subtract = ratings - 1
multiply = ratings * 2
divide = ratings / 2
exponent = ratings ** 2
```

---

### 1️⃣1️⃣ Universal Functions 🌍

```python
square_root = np.sqrt(ratings)
exponential = np.exp(ratings)
max_value = np.max(ratings)
sin_values = np.sin(ratings)
```

- `sqrt()` – Square root
- `exp()` – e^x
- `sin()` – Sine of elements

---

## 📈 Data Summary

```python
print("Shape:", numeric_data.shape)
print("Data Types:\n", numeric_data.dtypes)
print("Max per column:\n", numeric_data.max())
print("Min per column:\n", numeric_data.min())
print("Index of max value (Rating):", ratings.idxmax())
```

---

## ⚠️ FutureWarnings

You might see this:

```text
FutureWarning: 'Series.swapaxes' is deprecated
```

✅ Fix: Use `.values` or `.to_numpy()` for NumPy compatibility.

---

## 🗂️ File Structure

```
├── function.ipynb           # Main Notebook with all operations
├── IMDb_All_Genres.csv      # Cleaned Movie dataset
├── README.md                # Project summary (this file)
```

---

## ✅ How to Run

1. Open **Jupyter Notebook** via Anaconda
2. Run `function.ipynb`
3. Explore NumPy functionality applied to real movie data
4. Push project to GitHub 🚀

---

Enjoy exploring NumPy with real movie data! 🎥📊

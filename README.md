# NumPy Practice Notebooks

A collection of Jupyter notebooks covering the fundamentals of **NumPy**, built while learning Python for data science and machine learning. The notebooks move from creating arrays, to indexing and operations, to hands-on exercises that apply those concepts.

## Table of Contents

- [Notebooks](#notebooks)
- [Topics Covered](#topics-covered)
- [Exercises](#exercises)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)
- [Tech Stack](#tech-stack)

## Notebooks

| Notebook | Description |
|----------|-------------|
| [`Arrays.ipynb`](Arrays.ipynb) | Creating arrays, generation functions, random numbers, attributes, built-in methods, reshaping |
| [`array_indexing.ipynb`](array_indexing.ipynb) | Indexing and slicing of vectors and matrices, boolean indexing |
| [`array_OPERATIONS.ipynb`](array_OPERATIONS.ipynb) | Arithmetic operations, broadcasting, matrix operations, stacking and splitting |
| [`exercise.ipynb`](exercise.ipynb) | Practice problems: Sudoku validator and student marks analysis |

## Topics Covered

### 1. Array Basics (`Arrays.ipynb`)
- Creating arrays from Python lists (1D and 2D)
- Array generation: `np.arange()`, `np.zeros()`, `np.ones()`, `np.linspace()`
- Random generation: `np.random.rand()`, `np.random.randn()`, `np.random.randint()`
- Array attributes: `shape`, `size`, `dtype`
- Array methods: `min`, `max`, `sum`, `mean`, `std`, `argmin`, `argmax`
- Axis-wise operations (`axis=0` for columns, `axis=1` for rows)
- Reshaping arrays with `reshape()`

### 2. Indexing and Slicing (`array_indexing.ipynb`)
- Vector indexing and slicing, including reversing with `[::-1]`
- Matrix indexing: rows, columns, single elements, and sub-matrices
- Step slicing (e.g. `arr[::2]`)
- Boolean indexing to filter elements by condition

### 3. Operations and Manipulation (`array_OPERATIONS.ipynb`)
- Element-wise arithmetic: `+`, `-`, `*`, `/`, `//`, `**`
- Broadcasting with scalars and arrays
- Slices and copies
- Matrix multiplication with `@` and transpose with `.T`
- Stacking: `np.vstack()`, `np.hstack()`, `np.column_stack()`
- Splitting: `np.hsplit()`, `np.vsplit()`

## Exercises

`exercise.ipynb` applies the concepts above to two problems:

**Sudoku Validator**
Checks whether a 9x9 Sudoku grid is valid using NumPy only. Every row, every column, and every 3x3 sub-grid must sum to 45. Rows and columns are checked with `np.sum(..., axis=...)` and the 3x3 boxes with 2D slicing.

**Student Marks Analysis**
Works with a small dataset of student age, math marks, and science marks to practice:
- Finding the shape of the data and the average age
- Extracting a single column (math marks)
- Finding the highest science mark
- Filtering students with boolean conditions (e.g. math marks above 90, or at least 80 in both subjects)
- Updating values in place (adding 5 to all math marks, replacing low science marks with 0)
- Column-wise averages with `np.mean(..., axis=0)`

## Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
   cd YOUR-REPO-NAME
   ```

2. Install the dependencies:
   ```bash
   pip install numpy jupyter
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook
   ```

4. Open any `.ipynb` file and run the cells in order.

## Repository Structure

```
.
├── Arrays.ipynb
├── array_indexing.ipynb
├── array_OPERATIONS.ipynb
├── exercise.ipynb
└── README.md
```

## Tech Stack

- **Python**
- **NumPy**
- **Jupyter Notebook**

## Roadmap

- [ ] Pandas fundamentals
- [ ] Data visualization with Matplotlib
- [ ] More NumPy exercises and mini projects
- [ ] Introduction to machine learning with scikit-learn

## Author

**Jitender**

Feel free to open an issue or reach out if you have suggestions or feedback.

---

If you find this repository useful, consider giving it a star.

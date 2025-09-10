# MODULE-IV
## PYTHON SETUP FOR MATHEMATICAL AND SCIENTIFIC COMPUTING

### 1. Anaconda Installation Process
Anaconda is a free and open-source distribution of the Python and R programming languages for scientific computing. It aims to simplify package management and deployment, making it an essential tool for data scientists. The installation process is straightforward:
1.  **Download the Anaconda Installer:** Navigate to the official Anaconda website (anaconda.com/products/distribution) and download the installer for your operating system (Windows, macOS, or Linux).
2.  **Run the Installer:** Locate the downloaded file and run the installer. Follow the on-screen instructions. It is recommended to accept the default settings unless you have a specific reason to change them.
3.  **Add to PATH:** During installation, you will be asked whether you want to add Anaconda to your system's PATH environment variable. It is recommended to do this as it will make it easier to use Anaconda from the command line.
4.  **Launch Anaconda Navigator:** Once the installation is complete, you can launch the Anaconda Navigator, which is a graphical user interface (GUI) for managing your packages, environments, and launching applications like Jupyter Notebook and Spyder.
5.  **Conda Environments:** A key feature of Anaconda is `conda`, a package and environment manager. You can create isolated environments to manage dependencies for different projects. For example: `conda create --name myenv python=3.8`

### 2. Data Types with Python
Python has several built-in data types that are fundamental for storing and manipulating data. The most common data types are:
-   **Numeric Types:**
    -   `int`: Integer numbers (e.g., 10, -5, 0).
    -   `float`: Floating-point numbers (e.g., 3.14, -0.001).
    -   `complex`: Complex numbers (e.g., 1 + 2j).
-   **Sequence Types:**
    -   `list`: An ordered, mutable collection of items (e.g., `[1, 'apple', 3.14]`).
    -   `tuple`: An ordered, immutable collection of items (e.g., `(1, 'apple', 3.14)`).
    -   `range`: A sequence of numbers, commonly used for looping.
-   **Text Type:**
    -   `str`: A sequence of characters, used for text (e.g., `"Hello, World!"`).
-   **Mapping Type:**
    -   `dict`: An unordered collection of key-value pairs (e.g., `{'name': 'John', 'age': 30}`).
-   **Set Types:**
    -   `set`: An unordered collection of unique items (e.g., `{1, 2, 3}`).
    -   `frozenset`: An immutable version of a set.
-   **Boolean Type:**
    -   `bool`: Represents truth values, `True` or `False`.

### 3. Basic Operators and Setup
Python supports a wide range of operators for performing arithmetic, comparison, and logical operations.
-   **Arithmetic Operators:** `+` (addition), `-` (subtraction), `*` (multiplication), `/` (division), `%` (modulus), `**` (exponentiation), `//` (floor division).
-   **Comparison Operators:** `==` (equal to), `!=` (not equal to), `>` (greater than), `<` (less than), `>=` (greater than or equal to), `<=` (less than or equal to).
-   **Logical Operators:** `and` (logical AND), `or` (logical OR), `not` (logical NOT).

To get started with Python for data science, you will need to set up your development environment. This typically involves installing Python (which Anaconda does for you), a code editor or IDE (like VS Code, PyCharm, or Jupyter Notebook), and the necessary libraries (like NumPy, Pandas, and Matplotlib), which are also included in the Anaconda distribution.

### 4. Introduction to NumPy
NumPy (Numerical Python) is the fundamental package for scientific computing in Python. It provides a powerful N-dimensional array object, which is a grid of values, all of the same type. NumPy arrays are more efficient than Python lists for numerical operations. Key features include:
-   **`ndarray` object:** A fast and memory-efficient multidimensional array.
-   **Broadcasting:** A powerful mechanism that allows NumPy to work with arrays of different shapes when performing arithmetic operations.
-   **Vectorization:** The ability to perform batch operations on data without writing any `for` loops.
-   **Linear Algebra and Random Number Capabilities:** A comprehensive set of mathematical functions for linear algebra, Fourier analysis, and random number generation.

```python
import numpy as np

# Create a 1D NumPy array
a = np.array([1, 2, 3, 4, 5])
print(f"1D Array: {a}")

# Create a 2D NumPy array
b = np.array([[1, 2, 3], [4, 5, 6]])
print(f"2D Array:\n{b}")

# Basic array operations
print(f"Sum of array a: {np.sum(a)}")
print(f"Mean of array a: {np.mean(a)}")

# Vectorized operations
c = a * 2
print(f"Array a * 2: {c}")
```

### 5. Mathematical Functions of NumPy
NumPy provides a vast library of mathematical functions for performing element-wise operations on arrays. Some of the most common functions include:
-   **Trigonometric Functions:** `np.sin()`, `np.cos()`, `np.tan()`.
-   **Exponential and Logarithmic Functions:** `np.exp()`, `np.log()`, `np.log10()`.
-   **Rounding Functions:** `np.round()`, `np.floor()`, `np.ceil()`.
-   **Statistical Functions:** `np.mean()`, `np.median()`, `np.std()` (standard deviation), `np.var()` (variance), `np.sum()`, `np.min()`, `np.max()`.
-   **Array Manipulation:** `np.reshape()`, `np.transpose()`, `np.concatenate()`.

### 6. Introduction to SciPy
SciPy (Scientific Python) is a library that builds on NumPy and provides a large collection of algorithms and high-level functions for scientific and technical computing. While NumPy provides the basic array data structure, SciPy provides more specialized functions for a variety of scientific domains.

### 7. SciPy Packages
SciPy is organized into several subpackages, each of which corresponds to a different scientific computing domain. Some of the most important subpackages are:
-   `scipy.stats`: Contains a large number of probability distributions and a growing library of statistical functions.
-   `scipy.optimize`: Provides several optimization algorithms, including for function minimization, root finding, and curve fitting.
-   `scipy.integrate`: Provides tools for numerical integration, including ordinary differential equation solvers.
-   `scipy.linalg`: Contains linear algebra routines that are more extensive than those in NumPy.
-   `scipy.signal`: For signal processing tasks.
-   `scipy.sparse`: For sparse matrices and sparse linear system solvers.

### 8. Data Frame and Data Operations
A **DataFrame** is a 2-dimensional labeled data structure with columns of potentially different types, provided by the **pandas** library. You can think of it like a spreadsheet, a SQL table, or a dictionary of Series objects. It is the most commonly used pandas object and is central to data analysis in Python.
-   **Data Operations with pandas:** Pandas provides a rich set of functions for performing operations on DataFrames, such as:
    -   **Selection and Indexing:** Selecting rows, columns, and specific data points using labels (`.loc`) or integer positions (`.iloc`).
    -   **Filtering:** Filtering data based on conditions (e.g., `df[df['age'] > 30]`).
    -   **Sorting:** Sorting data by one or more columns (`.sort_values()`).
    -   **Grouping and Aggregation:** Grouping data by one or more columns and applying an aggregation function like `sum()`, `mean()`, or `count()` using the `.groupby()` method.
    -   **Handling Missing Data:** Dropping or filling missing values (`.dropna()`, `.fillna()`).
    -   **Merging and Joining:** Combining multiple DataFrames using database-style joins (`.merge()`, `.join()`).

```python
import pandas as pd

# Create a DataFrame from a dictionary
data = {'Name': ['Alice', 'Bob', 'Charlie', 'David'],
        'Age': [25, 30, 35, 40],
        'City': ['New York', 'Los Angeles', 'Chicago', 'Houston']}
df = pd.DataFrame(data)

print("DataFrame:")
print(df)

# Select a column
print("\nNames:")
print(df['Name'])

# Filter data
print("\nPeople older than 30:")
print(df[df['Age'] > 30])

# Group by a column and calculate the mean
print("\nAverage age by city:")
print(df.groupby('City')['Age'].mean())
```

### 9. Data Visualisation using Matplotlib
Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. It provides an object-oriented API for embedding plots into applications. It is highly customizable and is the foundation for many other plotting libraries in Python.
-   **Common Plots:**
    -   **Line Plot (`plt.plot()`):** To visualize the relationship between two continuous variables, often over time.
    -   **Scatter Plot (`plt.scatter()`):** To visualize the relationship and correlation between two numerical variables.
    -   **Histogram (`plt.hist()`):** To visualize the distribution of a single numerical variable by dividing the data into bins and counting the number of observations in each bin.
    -   **Bar Chart (`plt.bar()`):** To compare the values of different categories.
    -   **Box Plot (`plt.boxplot()`):** To visualize the distribution of a numerical variable through its quartiles and to identify outliers.
    -   **Pie Chart (`plt.pie()`):** To show the proportion of each category in a dataset.

```python
import matplotlib.pyplot as plt
import numpy as np

# Line Plot
x = np.linspace(0, 10, 100)
y = np.sin(x)
plt.plot(x, y)
plt.title("Sine Wave")
plt.xlabel("x")
plt.ylabel("sin(x)")
plt.show()

# Scatter Plot
x_scatter = np.random.rand(50)
y_scatter = np.random.rand(50)
plt.scatter(x_scatter, y_scatter)
plt.title("Scatter Plot")
plt.xlabel("x")
plt.ylabel("y")
plt.show()

# Histogram
data_hist = np.random.randn(1000)
plt.hist(data_hist, bins=30)
plt.title("Histogram")
plt.xlabel("Value")
plt.ylabel("Frequency")
plt.show()
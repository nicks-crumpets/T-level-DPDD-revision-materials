# Pandas

# Key features

- Fast data loading
- Data manipulation, alignment and merging

## Qualitative and quantitative data

Qual is descriptive quan is numbers (less needed?)

# Data representation in pandas

Quantitative data in pandas:

- Stores as numeric types (int, float etc)
- Supports operations such as mean median and standard division

Qualitative data in pandas:

- Stored in categories or objects (str)
- —

## Converting qualitative into quantitative

### Sentiment analysis

- E.g: Analysing customer reviews for a product on an online store

- Qualitative: “This is amazing!”
- Conversion: Assign a Positive sentiment score
- —
- —
    - —
    - —
    - —

One-Hot encoding

Ordinal encoding

# Code

### Importing pandas

```python
import pandas as df
```

### Dataset shape

```python
print(df.shape)
```

```
(1704, 6)
```

### Dataset start & end

```python
# prints the first and last 5 rows of data
print(df.head())
print(df.tail())
```

```
country continent  year  lifeExp       pop   gdpPercap
0  Afghanistan      Asia  1952   28.801   8425333  779.445314
1  Afghanistan      Asia  1957   30.332   9240934  820.853030
2  Afghanistan      Asia  1962   31.997  10267083  853.100710
3  Afghanistan      Asia  1967   34.020  11537966  836.197138
4  Afghanistan      Asia  1972   36.088  13079460  739.981106
       country continent  year  lifeExp       pop   gdpPercap
1699  Zimbabwe    Africa  1987   62.351   9216418  706.157306
1700  Zimbabwe    Africa  1992   60.377  10704340  693.420786
1701  Zimbabwe    Africa  1997   46.809  11404948  792.449960
1702  Zimbabwe    Africa  2002   39.989  11926563  672.038623
1703  Zimbabwe    Africa  2007   43.487  12311143  469.709298
```

### Show column datatypes

```python
print(df.dtypes)
```

```
country       object
continent     object
year           int64
lifeExp      float64
pop            int64
gdpPercap    float64
dtype: object
```

### —

New data.csv file

### Data correlations

```python
print(df.corr())
```

```
          Duration     Pulse  Maxpulse  Calories
Duration  1.000000 -0.155408  0.009403  0.922717
Pulse    -0.155408  1.000000  0.786535  0.025121
Maxpulse  0.009403  0.786535  1.000000  0.203813
Calories  0.922717  0.025121  0.203813  1.000000
```

### Plotting

**Standard graph**

```python
import matplotlib.pyplot as plt

df = pd.read_csv('data.csv')

df.plot()

plt.show()
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image.png)

**Histogram**

```python
df["Duration"].plot(kind = 'hist')
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%201.png)

**Scatter**

```python

df.plot(kind = 'scatter', x = 'Duration', y = 'Maxpulse')
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%202.png)

# Matplotlib Pyplot

### Import

This applies to all code under this title

```python
import matplotlib.pyplot as plt
import numpy as np
```

### Drawing an upward linear line

```python

xpoints = np.array([0, 6])
ypoints = np.array([0, 250])

plt.plot(xpoints, ypoints)
plt.show()
```

### Plotting a line from pos (1,3) to pos (8,10)

```python
xpoints = np.array([1, 8])
ypoints = np.array([3, 10])

plt.plot(xpoints,ypoints)
plt.show()
```

![This is the correct points, the axis automatically adjusts](Pandas%201a45301291278029bb4ac88db2d93111/image%203.png)

This is the correct points, the axis automatically adjusts

### Plotting 2 points at (1, 3) and (8, 10)

```python
xpoints = np.array([1, 8])
ypoints = np.array([3, 10])

plt.plot(xpoints,ypoints, 'o')
plt.show()
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%204.png)

### Plotting a line from (1, 3) to (2, 8) to (6, 1)

```python
xpoints = np.array([1, 2, 6, 8])
ypoints = np.array([3, 8, 1, 10])

plt.plot(xpoints,ypoints)
plt.show()
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%205.png)

### Demonstration of default X-points

```python
ypoints = np.array([3, 8, 1, 10, 5, 7])

plt.plot(ypoints)
plt.show()
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%206.png)

### Marking each point with a plot point

```python
plt.plot(ypoints, marker = 'o')
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%207.png)

Or, mark with an ‘X’

```python
plt.plot(ypoints, marker = 'o')
```

![image.png](Pandas%201a45301291278029bb4ac88db2d93111/image%208.png)

Marker 	Description
'o' 	Circle 	
'*' 	Star 	
'.' 	Point 	
',' 	Pixel 	
'x' 	X 	
'X' 	X (filled) 	
'+' 	Plus 	
'P' 	Plus (filled) 	
's' 	Square 	
'D' 	Diamond 	
'd' 	Diamond (thin) 	
'p' 	Pentagon 	
'H' 	Hexagon 	
'h' 	Hexagon 	
'v' 	Triangle Down 	
'^' 	Triangle Up 	
'<' 	Triangle Left 	
'>' 	Triangle Right 	
'1' 	Tri Down 	
'2' 	Tri Up 	
'3' 	Tri Left 	
'4' 	Tri Right 	
'|' 	Vline 	
'_' 	Hline
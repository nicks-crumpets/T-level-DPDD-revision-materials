# Bob's Taxis practice

## Starting imports & reading

```python
import pandas as pd
import matplotlib.pylot as plt

df = pd.read_csv("bobs_taxis.csv")
```

## Displaying the ‘header’ of the data

```python
print(df.head(5))
```

## Display info about the dataset

```python
print(df.info())
```

## Filter data frame by a value in a column

```python
**filtered = df[df['pickup_month'] == 1]
print(filtered)**
```

## Show number of rows in filtered dataset

```python
filtered = df[df['pickup_month'] == 1]
print(filtered.shape[0])
```

## Top *X* values in a column

```python
n = 5
# prints the top 5 values and how many times they occur
frequency_multiple = df['pickup_location_code'].value_counts()[:n]
print(frequency_multiple)
```

## Compare two columns data

```python
comparison = df[['trip_distance', 'fare_amount']]

comparison.plot(kind='scatter', x='fare_amount', y='trip_distance')
plt.show()
```
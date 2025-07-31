# Melt

Melt is a useful function inside pandas that helps to simplify data, making it easier to just look at and most importantly to make graphs

Original data used for these examples

[DAT.csv](Melt%201e653012912780989531d4f986a5664f/DAT.csv)

# How to simplify some data

```python
df = pd.read_csv("DAT.csv")

tidy = df.melt(
	id_vars=["Menu Item", "Service"],
	var_name="Date",
	value_name="Portions")

tidy["Date"] = pd.to_datetime(tidy["Date"], dayfirst=True)

print(tidy.head(25))
```

This displays…

```
   Menu Item Service       Date  Portions
0     Nachos   Lunch 2023-03-03        23
1       Soup   Lunch 2023-03-03        40
2     Burger   Lunch 2023-03-03        25
3    Brisket   Lunch 2023-03-03        25
4       Ribs   Lunch 2023-03-03        41
5       Corn   Lunch 2023-03-03        14
6      Fries   Lunch 2023-03-03         5
7      Salad   Lunch 2023-03-03        33
8     Nachos  Dinner 2023-03-03        59
9       Soup  Dinner 2023-03-03         8
10    Burger  Dinner 2023-03-03        13
11   Brisket  Dinner 2023-03-03        46
12      Ribs  Dinner 2023-03-03         7
13      Corn  Dinner 2023-03-03        48
14     Fries  Dinner 2023-03-03        46
15     Salad  Dinner 2023-03-03        59
16    Nachos   Lunch 2023-03-04        33
17      Soup   Lunch 2023-03-04        14
18    Burger   Lunch 2023-03-04        35
19   Brisket   Lunch 2023-03-04         3
20      Ribs   Lunch 2023-03-04         9
21      Corn   Lunch 2023-03-04        14
22     Fries   Lunch 2023-03-04        35
23     Salad   Lunch 2023-03-04         6
24    Nachos  Dinner 2023-03-04        11

Process finished with exit code 0
```

# Graphs using melt

**!! Keeping the code from the previous section !!** Let’s add some code to make a graph

This is going to display a line graph of ‘portions’ per day

```python
# Changes the date formatting so that it displays correctly for graphs
tidy["Date"] = pd.to_datetime(tidy["Date"], dayfirst=True)

# groups the data by the date, calculates the sun of portions for each date
daily_totals = tidy.groupby("Date")["Portions"].sum()

# Previous data with all modifications, sets it to a line chart with a specified title
daily_totals.plot(kind="line", title="Total Portions sold per day")

# y axis label
plt.ylabel("Portions")

# Grid setting
plt.grid(True)

# Shows the plot
plt.show()
```

And that should display…

![image.png](Melt%201e653012912780989531d4f986a5664f/image.png)

# A bit more complicated melted graphs

Now it’s time to try splitting the portions into if they were served for Lunch, or for Tea/Dinner

**!! Keep the first code block only !!**

```python
# This code creates a line graph comparing the lunch and dinner sales
service_trend = tidy.groupby(["Date", "Service"])["Portions"].sum().unstack()

# Prints the first few rows to demonstrate how the data is formatted
print(service_trend.head(25))

# Sets a title and type of chart
service_trend.plot(title="Lunch VS Tea sales")

# Sets y axis label
plt.ylabel("Portions")

# sets x axis label
plt.xlabel("Date")

# Rotates number values on x-axis a set amount of degrees
plt.xticks(rotation=45)

# Keeps everything tighter together so that areas are not cut odd
plt.tight_layout()

# Shows graph
plt.show()
```

And this displays…

![image.png](Melt%201e653012912780989531d4f986a5664f/image%201.png)

---

Here is how the data looks like in a table, it’s easier to navigate in a spreadsheet program or inside PyCharm

[Restaurant data](Melt%201e653012912780989531d4f986a5664f/Restaurant%20data%201e653012912780279b6efdf212779205.csv)
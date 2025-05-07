- How do you use melt on a dataset to make it easier to read? >>>
    - .
        ```
        tidy = df.melt(
    id_vars=["ID's TO", "NOT MOVE"],
    var_name="DATE",
    value_name="VALUES LISTED UNDER DATES")
    
tidy["DATE"] = pd.to_datetime(tidy["DATE"], dayfirst=True)
        ```
- How to group 2 elements so they can be displayed in a graph after tidying the data? (This example is grouping the dates with the main data) >>>
    - .
        ```
        VAR = MELT_VAR("DATE")["THINGS"].sum
        ```
    - Note that the `THINGS` should be the same name given to the data to move around as you have in the code previously, otherwise it won't work
- When the data is in an acceptable state to plot on a graph, how do you plot it on a graph? >>>
    - .
        ```
        DATA.plot(kind="GRAPH_KIND_HERE", title"TITLE_OF_GRAPH")

plt.ylabel("Y_AXIS_LABEL")

plt.ylabel("X_AXIS_LABEL")

plt.show() 
        ```
- How do you split data to compare two sections of data (e.g. AM sales versus PM sales)? >>>
    - .
        ```
        VAR = MELT_VAR.groupby(["DATE", "DIFFERING_COLUMN"])["THINGS"].sum().unstack
        ```
    - The `DIFFERING_COLUMN` is the column that shows what data is attributed to what section, for example when doing AM vs PM sales, the column that says AM or PM
- How do you rotate the text for the x-axis labels?→`plt.xticks(rotation=45)` 
- What are the three variables you need to use when melting data and what needs to be placed inside them? >>>
    - `id_vars` - This is where all columns that should NOT move go, such as the menu items or a flight code that's not the actual data
    - `var_name` - The name given the the column headers above the data when they're pushed into their own column
    - `value_name` - Name for the actual data, such as the passengers on a plane, or sausages sold. This name doesn't display when just printing the tidied dataset, but just gives a name for the data to be stored under
- 
- 

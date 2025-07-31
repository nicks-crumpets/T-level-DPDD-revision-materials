# Cleaning data

Removing duplicates, extra spaces, and correcting missing/inaccurate data 

Also known as manipulating it, as it requires modification of the data

You need to know the data well, otherwise manipulating it can damage its integrity

## Replacing data

For example, with an old film, if scenes are broken or missing…

Can take a large amount of time

- Finding & removing duplicate data
- Finding & removing extra characters
- Separating data without deliminators

## Removing duplicate data

One of the first things that should be done when cleaning data

Duplicate data isn’t just data that is the same

For example a sales dataset may have many of the same product

A duplication is if an *entire record* is duplicated

### Leading & trailing spaces

Both spaces and tabs are invisible to people but have a value to a computer

However it means a dataset may have duplicate records, because 2 records that are the same,  but one has spaces, will be seen as completely different records

## Separating data

Some data may need separation, or removing separation

For example, with a phone number, some users may enter it with no spaces, and some may separate a country code away from the main number. Meaning it needs modification in order to work in the dataset

## Correcting inaccurate data

Data that doesn't make sense or that will cause errors or problems during an analysis

To know weather or not data is accurate, there needs to be a good knowledge of the data

For example, when entering the current date, a user may use an incorrect or different date format, if not caught by error checking (which it should be) it needs to be changed or removed

The day and year may be switched in dates by accident, known as a transposition error 

## Missing data

Lots in common with inaccurate data, and therefore the data needs to be known well in order to

Fixing this is known as imputation

- Average/Mean filling - Replaces it with a column average, simple and quick and also works best for normally distributed data
- Forward fill/Propagation - Copies last known value to missing entry, ideal for time series or sequential data
- Backward fill - Copies the previous value into missing entry
- Linear interpolation

# Standardising text data

Case normalisation

- All text to lowercase
- Eliminates case-sensitive variations
- Test → TEST → tEsT → test

Uppercase conversion

- Less common but used in specific cases
- Consistent uppercase representation

Special character treatment

- Removes any special characters
- Standardises text

## Formatting dates

They must be in one standard format, global is YYYMMDD, but can be country specific, usually not preferred due to the likely confusion 

## Working with outliers

Data that is valid, but outside what is considered the standard range of the data

Outliers can cause something known as **skewing** because if you have an extremely large piece of data

This can be fixed by

- Removing the outlier
- Removing the outlier and stating the upper range
- Finding the median

## Visualising the data

Putting the data into a chart or graph to see patterns, trends etc much more clearly
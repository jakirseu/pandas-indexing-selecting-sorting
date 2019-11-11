# Python Pandas Indexing Selecting & Sorting
Python Pandas indexing, sorting, selecting etc demo. 

In this demo, we used [Irish Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv). 
  
## Printing all items from a column

    print(df['sepal_length'])  

  
##  Printing single items from a column  

    print('first items of sepal_length column ')  
    print(df['sepal_length'][0])  

  
## Print all columns  from a dataframe

    print('all columns of dataframe')  
    print(df.columns)  

  
## Printing first row of dataframe  

    print('first row of dataframe')  
    print(df.iloc[0])  

  
## Printing second row of dataframe  

    print('second row of dataframe')  
    print(df.iloc[1])  

  
## Printing a column using loc  

    print('printing all items from sepal_length or 0 index')  
    print(df.iloc[:, 0])  

  
## Printing a column using loc  

    print('printing all items from sepal_width or 1 index')  
    print(df.iloc[:, 1])  

  
  
## Printing 5 items from a column using loc  

    print('printing 5 items from sepal_length or 0 index')  
    print(df.iloc[:5, 0])  

  
  
## Printing a column using iloc  

    print('printing all items from sepal_length')  
    print(df.loc[:,'sepal_length'])  

  
  
## Printing all items from selected columns  

    print('printing selected columns')  
    print(df[['sepal_length', 'sepal_width']])  

  
## Getting summary value from a column  

    print('summaries from a column')  
    print(df['sepal_length'].max())  
    print(df['sepal_length'].min())  
    print(df['sepal_length'].mean())  

  
## Conditional selection  

    print('conditional selections')  
    print(df[df['sepal_width'] >4])  
    print(df['sepal_width'][df['sepal_width'] >4])  
    print(df[(df['sepal_width'] >3) &  (df['sepal_length'] >=6)])  

  
## Sorting  

    print('sorting dataframe by a column')  
    print(df.sort_values(by='sepal_length'))  
    print(df.sort_values(by='sepal_length', ascending=False))

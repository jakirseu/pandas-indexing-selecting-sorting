# Python Pandas Indexing Selecting & Sorting
Python Pandas indexing, sorting, selecting etc demo. 

In this demo, we used [Irish Dataset](https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv). 
  
## printing all items from sepal_length  

    print(df['sepal_length'])  

  
##  printing single items from sepal_length  

    print('first items of sepal_length column ')  
    print(df['sepal_length'][0])  

  
## print all columns  

    print('all columns of dataframe')  
    print(df.columns)  

  
## printing first row of dataframe  

    print('first row of dataframe')  
    print(df.iloc[0])  

  
## printing second row of dataframe  

    print('second row of dataframe')  
    print(df.iloc[1])  

  
## printing a column using loc  

    print('printing all items from sepal_length or 0 index')  
    print(df.iloc[:, 0])  

  
## printing a column using loc  

    print('printing all items from sepal_width or 1 index')  
    print(df.iloc[:, 1])  

  
  
## printing 5 items from a column using loc  

    print('printing 5 items from sepal_length or 0 index')  
    print(df.iloc[:5, 0])  

  
  
## printing a column using iloc  

    print('printing all items from sepal_length')  
    print(df.loc[:,'sepal_length'])  

  
  
## getting selected columns  

    print('printing selected columns')  
    print(df[['sepal_length', 'sepal_width']])  

  
## getting summary value from a column  

    print('summaries from a column')  
    print(df['sepal_length'].max())  
    print(df['sepal_length'].min())  
    print(df['sepal_length'].mean())  

  
## conditional selection  

    print('conditional selections')  
    print(df[df['sepal_width'] >4])  
    print(df['sepal_width'][df['sepal_width'] >4])  
    print(df[(df['sepal_width'] >3) &  (df['sepal_length'] >=6)])  

  
## sorting  

    print('sorting dataframe by a column')  
    print(df.sort_values(by='sepal_length'))  
    print(df.sort_values(by='sepal_length', ascending=False))

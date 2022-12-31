

Q1. How do you load a CSV file into a Pandas DataFrame?

  -> We can load a csv file into pandas dataframe using below commands
  	df = pd.read_csv("https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv")
	df
	
Q2. How do you check the data type of a column in a Pandas DataFrame?

  -> df.dtypes command is used to check the datatype of a column in pandas dataFrame
  
Q3. How do you select rows from a Pandas DataFrame based on a condition?

  -> we can use loc and iloc function to select rows from a pandas Dataframe based on different conditions.
  
Q4. How do you rename columns in a Pandas DataFrame?

  -> rankings = {'test': ['India', 'South Africa', 'England',
                            'New Zealand', 'Australia'],
            'odi': ['England', 'India', 'New Zealand',
                            'South Africa', 'Pakistan'],
            't20': ['Pakistan', 'India', 'Australia',
                            'England', 'New Zealand']}
	rankings_pd = pd.DataFrame(rankings)
	print(rankings_pd)
	rankings_pd.rename(columns = {'test':'TEST'}, inplace = True)
	
Q5. How do you drop columns in a Pandas DataFrame?

  -> We can use drop() function to drop any column in pandas DataFrame
    for eg - df.drop('t20', axis=1,inplace = True)
    
Q6. How do you find the unique values in a column of a Pandas DataFrame?

  -> unique() method is used to get the unique values of a column in pandas DataFrame.
     for eg - print(rankings_pd['odi'].unique())
     
Q7. How do you find the number of missing values in each column of a Pandas DataFrame?

  -> First we can use isnull() function to check the missing values in a column.
     furthermore by using sum() function with the isnull() function we can get the total number of missing values in a column.
     for eg - df.isnull().sum()
     
Q8. How do you fill missing values in a Pandas DataFrame with a specific value?

  -> The fillna() method can be used to fill the null or missing values in a pandas Dataframe with a specified value.
     for eg - syntax of fillna() - dataframe.fillna(value, method, axis, inplace)
     
Q9. How do you concatenate two Pandas DataFrames?

  -> concat() method can be used to concat two dataframes in pandas.
    for eg - frames = [df_con1,df_con2]
    df_new = pd.concat(frames)
    df_new
    
Q10. How do you merge two Pandas DataFrames on a specific column?

  -> merge() function can be used to merge two dataframes in Pandas.
  for eg - df7.merge(df6[[ 'Name', 'Marks']],on = 'Name', how = 'left')
  
Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?

  -> We can use groupby() function to group data in a Pandas DataFrame by a specific column and then use any aggregation function along with it to get the desired output.
  for eg - print(df.groupby('Name').groups)
  	   sum_gk = df.groupby(['Name']).sum()
  	   sum_gk
  	   
Q12. How do you pivot a Pandas DataFrame?

  -> We can use pivot() method to pivot the data in a Pandas DataFrame.
   	 syntax - df.pivot('A', 'B', 'C')
  	  A, B and C are the parameters to be passed in the pivot() function
  	  Parameters:
  	  index[ndarray] : Labels to use to make new frame’s index
  	  columns[ndarray] : Labels to use to make new frame’s columns
  	  values[ndarray] : Values to use for populating new frame’s values
  	  for eg -
  	  df.pivot('Name','Age','Address')
  	  
Q13. How do you change the data type of a column in a Pandas DataFrame?

  -> The astype() method is used to cast pandas object to a specified dtype.
     This function also provides the capability to convert any suitable existing column to a categorical type.
     for eg - df = df.astype(str)
     print(df.dtypes)
  
Q14. How do you sort a Pandas DataFrame by a specific column?

  -> To sort the DataFrame based on the values in a single column, We will use .sort_values().
     By default, this will return a new DataFrame sorted in ascending order. It does not modify the original DataFrame.
     for eg - so=df.sort_values('Age')
     
Q15. How do you create a copy of a Pandas DataFrame?

  -> The copy() method returns a copy of the DataFrame.
     By default, the copy is a "deep copy" meaning that any changes made in the original DataFrame will NOT be reflected in the copy.
     for eg - newdf=df.copy(deep=True)
	      display(df)
	      display(newdf)
	     
Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?

  -> We can use loc method to filter rows of a Pandas Dataframe by multiple conditions.
     for eg - samp_data = pd.DataFrame({'Name': [' RACHEL  ', ' MONICA  ', ' PHOEBE  ',
                                   '  ROSS    ', 'CHANDLER', ' JOEY    '],
                           
                          'Age': [30, 35, 37, 33, 34, 30],
                           
                          'Salary': [100000, 93000, 88000, 120000, 94000, 95000],
                           
                          'JOB': ['DESIGNER', 'CHEF', 'MASUS', 'PALENTOLOGY',
                                  'IT', 'ARTIST']})
		display(samp_data.loc[(samp_data['Salary']>=100000) & (samp_data['Age']< 40) & (samp_data['JOB'].str.startswith('D')),['Name','JOB']])
		
Q17. How do you calculate the mean of a column in a Pandas DataFrame?

  -> The mean() method can be used to find the mean value of a column in a Pandas DataFrame.
     for eg - pd.DataFrame({"A":[12, 4, 5, None, 1],
                   "B":[7, 2, 54, 3, None],
                   "C":[20, 16, 11, 3, 8],.
                   "D":[14, 3, None, 2, 6]})
              mdata.mean(axis=0)
              
Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?

  -> Standard deviation is calculated using the function .std().
     However, the Pandas library creates the Dataframe object and then the function .std() is applied on that Dataframe.
     for eg - answer= df.std()
     
Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?

  -> By using corr() function we can get the correlation between two columns in the dataframe.
     for eg - dataset.corr()
     
Q20. How do you select specific columns in a DataFrame using their labels?

  -> We Use DataFrame.loc[] and DataFrame.iloc[] to select a single column or multiple columns from pandas DataFrame by column names/label or index position respectively.
     where loc[] is used with column labels/names and iloc[] is used with column index/position.
     
Q21. How do you select specific rows in a DataFrame using their indexes?

  -> We can select a single row from pandas DataFrame by integer index using df.iloc[n]. Replace n with a position you wanted to select.
     for eg - print(df.iloc[2])
              print(df.iloc[2:6])
              
Q22. How do you sort a DataFrame by a specific column?

  -> To sort the DataFrame based on the values in a single column, We will use .sort_values().
     By default, this will return a new DataFrame sorted in ascending order. It does not modify the original DataFrame.
     for eg - so=df.sort_values('Age')
     
Q23. How do you create a new column in a DataFrame based on the values of another column?

  -> We can create a new column in a pandas dataframe by combining the values of two data columns by using below syntax.
     for eg - df['new_col'] = df['Survived'] + df['Pclass']
              df.head()
    
Q24. How do you remove duplicates from a DataFrame?

  -> The drop_duplicates() method removes duplicate rows.
     Use the subset parameter if only some specified columns should be considered when looking for duplicates.
     for eg - newdf = df.drop_duplicates()

Q25. What is the difference between .loc and .iloc in Pandas?

  -> We Use DataFrame.loc[] and DataFrame.iloc[] to select a single column or multiple columns from pandas DataFrame by column names/label or index position respectively.
     where loc[] is used with column labels/names and iloc[] is used with column index/position.
    
   
    
    
    
    
    
    
    
    
    
    
    

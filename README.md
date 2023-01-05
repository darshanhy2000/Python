# Python Left join two CSV file 

import pandas as pd

# reading csv files
statement_1 = pd.read_csv('statement_1.csv')
statement_2= pd.read_csv('statement_2.csv')

# using merge function by setting how=
output3 = pd.merge(statement_1,statement_2,
				 on='LID_No',
				how='right')

# displaying result
print(output3)

# Pandas
import pandas as pd 
import numpy as np
from numpy import random
# Series Creation
ser1 = pd.Series(data=random.randint(10,45,size=5),
index=['a','b','c','d','e']) 
print("Series is")
print(ser1)
#DataFrame Creation
df = pd.DataFrame(data=np.arange(101,126).reshape(5,5),
index=['A','B','C','D','E'],
columns=['U','V','W','X','Y'])
print("Data frame is") 
print(df)
print("Column wise accessing") 
print(df['W']['A']) 
print(df['W']) 
print(df[['W','X','U']])
print("Row wise accsessing") 
print(df.loc['A']['X']) 
print(df.loc['B']) 
print(df.loc[['B','A']])
print(df.iloc[2]['X']) 
print(df.iloc[1]) 
print(df.iloc[2:4])

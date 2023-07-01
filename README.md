# OldFaithful
Old Faithful is a cone geyser in Yellowstone National Park in Wyoming, United States. It was named in 1870 during the Washburn–Langford–Doane Expedition and was the first geyser in the park to be named. It is a highly predictable geothermal feature and has erupted every 44 minutes to two hours since 2000.
<br>
<br>
Let's import pandas, and matplotlib to do some basic analysis on the data and make a few visualizations.
<br>
<br>
import pandas as pd
import matplotlib as plot
%matplotlib inline
<br>
<br>
df=pd.read_csv('https://raw.githubusercontent.com/CunyLaguardiaDataAnalytics/datasets/master/faithful.csv', index_col=0)
<br>
<br>
df.head    shows us the first 5 rows
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/cef80912-86eb-4ca5-be80-8b81f7d979c6)
<br>
<br>
df.tail()    shows us the last 5 rows
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/6a6d57af-e643-4978-83bf-fa480b038202)
<br>
<br>
df.head(10)     shows us the first 10 rows
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/1eeef691-60a2-4252-af3f-d5372e1d4634)
<br>
<br>
df.count()     counts the total amount of entries in each column
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/7666dcf9-0fbf-406f-b5c3-34dc88a6a289)
<br>
<br>
df.max()     shows the maximum value of the columns
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/5a151a5d-8bea-4d9e-815f-66b302f9e81f)
<br>
<br>
df.min()    shows the minimum value of the columns
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/9a96ccbf-032c-489d-8131-f44295d58abc)
<br>
<br>
df.mean()      shows the mean or average of each column
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/8ea6ffba-fcd4-4c0f-b680-fb2c0ca3aa6f)
<br>
<br>
df.median()
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/644994fe-8f41-4279-a35b-7df3dec2de19)
<br>
<br>
df.describe()      shows a general statistics description of the columns
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/e4e25c19-9ec5-43f8-9d10-be8cfe3a4318)
<br>
<br>
If we use the .mean method for a specific column, we get the same result as the general statistics description above.
<br>
<br>
df['eruptions'].mean()
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/317d8f0c-c757-45f4-b4b4-738536c83a9f)
<br>
<br>
Let's create basic visualizations using matplotlib
<br>
<br>
See below a Histogram made from our dataframe df
<br>
<br>
df.hist()
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/56b1e811-1fe0-4bb8-ae58-16a065768456)
<br>
<br>
df.plot()
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/2c031297-1377-45e2-9388-c8de11429f94)
<br>
<br>
df.plot(kind='hist')
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/5af54080-dcab-4b1f-8795-13795ed7fc28)
<br>
<br>
df.plot(kind='scatter',x='waiting',y='eruptions')
<br>
<br>
![image](https://github.com/marcosalinas777/OldFaithful/assets/95108103/3d8403b4-5646-4d44-a0bc-5afe055cdee6)




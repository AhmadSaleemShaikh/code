Read csv file

import pandas as pd
import matplotlib.pyplot as plt

# reading the database
data=pd.read_csv("AAPL.csv")

# printing the top 10 rows
print(data.head(10))

# print first 5 and last 5
#print(data)

print(data.tail(3))
print(data.describe())
plt.plot(data['Date'],data['Close'])
plt.show()


import csv

with open('tips.csv','r')as file:
    reader=csv.reader(file)
    for row in reader:
        print(row)

Line Graph

#import numpy as np
import matplotlib.pyplot as plt
year = [2010, 2011, 2012, 2013, 2014, 2015]
yeild_apple = [0.895, 0.91, 0.919, 0.926, 0.929, 0.930]
plt.plot(year,yeild_apple )
plt.plot(year,yeild_apple ,marker='o')
plt.title("Line Graph")
plt.xlabel('Years')
plt.ylabel('Yeild (in hecter)')
plt.show()


Multiple Line Graph

#import numpy as np
import matplotlib.pyplot as plt
year = [2010, 2011, 2012, 2013, 2014, 2015]
yeild_apple = [0.895, 0.91, 0.919, 0.926, 0.929, 0.930]
oranges =[0.962, 0.941, 0.930, 0.923, 0.918, 0.908]
plt.plot(year,yeild_apple )
plt.plot(year,oranges)
plt.title(" Multiple Line Graph")
plt.xlabel('Years')
plt.ylabel('Yeild (in hecter)')
plt.show()

Bar chart

#import numpy as np
import matplotlib.pyplot as plt
year = [2010, 2011, 2012, 2013, 2014, 2015]
yeild_apple = [0.895, 0.91, 0.919, 0.926, 0.929, 0.930]
oranges =[0.962, 0.941, 0.930, 0.923, 0.918, 0.908]
plt.plot(year,yeild_apple )
plt.plot(year,oranges)
plt.title(" Multiple Line Graph")
plt.xlabel('Years')
plt.ylabel('Yeild (in hecter)')
plt.show()

Scatter Plot

#import numpy as np
import matplotlib.pyplot as plt
year = [2010, 2011, 2012, 2013, 2014, 2015]
yeild_apple = [0.895, 0.91, 0.919, 0.926, 0.929, 0.930]
plt.bar(year,yeild_apple )
plt.title("BAR PLOT")
plt.xlabel('Years')
plt.ylabel('Yeild (in hecter)')
plt.show()

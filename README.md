# Visualization
import numpy as np
import matplotlib.pyplot as plt

heights=[10,15,20,25,30]
names=['Derry','Evans','Deborah','Yeng','Rashid']

y_lable=np.arange(len(names))

plt.bar(y_lable,heights)
plt.xticks(y_lable,names)
plt.show()


#student Performance Analysis
data=pd.read_csv("StudentsPerformance.csv")
df=pd.DataFrame(data)
read=df['Reading score'].values
write=df['Writing score'].values
maths=df['Math score'].values
race=df['Race/Ethnicity'].values
z=np.array(maths)
gender=df.Gender.values
y=np.array(write)
lists=list(y)
x=np.array(read)
readMean =x.mean()
writemean=y.mean()
def hists():
  plt.hist(x, bins='auto',color='red')
  plt.legend("Simple graph")
  plt.text(21,95,r'%mean=69.169, b=3%')
  plt.show()
def Line():
  plt.plot(y,'g^')
  plt.ylabel("Line graph")
  plt.show()

def bars():
  plt.bar(gender,x)
  plt.title("Bar graph")
  plt.show()
  maths.flatten()
A=df.groupby("Gender")
A.first()
A.last()
meanG=A.mean()
meanG




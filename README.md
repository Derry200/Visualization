# Visualization
import numpy as np
import matplotlib.pyplot as plt

heights=[10,15,20,25,30]
names=['Derry','Evans','Deborah','Yeng','Rashid']

y_lable=np.arange(len(names))

plt.bar(y_lable,heights)
plt.xticks(y_lable,names)
plt.show()



import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
ax = plt.gca()

data.plot(kind='line',x='Date',y='Qt,(MMscf/day)',ax=ax)
data.plot(kind='line',x='Date',y='Gp(t),MMscf/day)',ax=ax,color='red',marker='o')
plt.title('Decline curve analysis')
plt.xlabel('Date')
plt.ylabel('Gp/Qt')
fig_size = plt.rcParams["figure.figsize"]
fig_size[0] = 15
fig_size[1] = 5
plt.rcParams["figure.figsize"] = fig_size
plt.show()

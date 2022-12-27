#I am importing libraries and datasets with death causes in the US and EU by most common.

import matplotlib.pyplot as plt
import pandas as pd
import numpy as np

US_data = pd.read_csv('C:/Users.../Data US - death causes.csv', sep=';')
EU_data = pd.read_csv('C:/Users.../Data EU - death causes.csv', sep=';')

#After that, I am performing some typical data transformations, such as creating subsets and labeling.

US_subset = US_data.iloc[0, 0:10]
US_subset2 = US_data.values.sum()
EU_subset = EU_data.iloc[0, 0:8]
US = US_subset.div(US_subset2)
labels = US_data.columns
explode = [0.15] * 10
textprops = {"fontsize": 11}

#I am creating a pie chart of the most common death causes in the US and EU.

plt.pie(x=US_subset, labels=labels, shadow=True, autopct='%.1f%%', radius=1.2, pctdistance=0.75, wedgeprops={"edgecolor": "black", 'linewidth': 1, 'antialiased': True}, explode=explode, textprops=textprops)
circle = plt.Circle(xy=(0, 0), radius=0.5, facecolor='white', edgecolor="k", linewidth=1.5)
plt.gca().add_artist(circle)
plt.show()



labels2 = EU_data.columns
explode2 = [0.15] * 8
textprops = {"fontsize": 11}
plt.pie(x=EU_subset, labels=labels2, shadow=True, autopct='%.1f%%', radius=1.2, pctdistance=0.75, wedgeprops={"edgecolor": "black", 'linewidth': 1, 'antialiased': True}, explode=explode2, textprops=textprops)
circle = plt.Circle(xy=(0, 0), radius=0.5, facecolor='white', edgecolor="k", linewidth=1.5)
plt.gca().add_artist(circle)
plt.show()

#I am setting everything up for the next plot, which will be made up of multiple plots.

fig, ax = plt.subplots(3)
ax[0].plot(DRG_returns, antialiased=True)
ax[0].set_ylabel('DRG_returns')
ax[1].plot(SP500_returns, color='red', antialiased=True)
ax[1].set_ylabel('SP500_returns')
ax[2].plot(EU_returns, color='green', antialiased=True)
ax[2].set_ylabel('EU_returns')
plt.show()


print(np.std(DRG_returns), np.std(SP500_returns), np.std(EU_returns))

#The standard deviation values indicate that there is not a significant difference in risk exposure.
#Pharma index: 0.027
#US - SP500: 0.038
#EU - Euronext: 0.047


#Based on this information, my recommendation is to invest in the production of circulatory system and cancer medicines on the US and European markets.
#However, the company should also plan additional business activities to be consistent on the market due to the high level of economic uncertainty.





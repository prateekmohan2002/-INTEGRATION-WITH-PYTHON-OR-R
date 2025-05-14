# -INTEGRATION-WITH-PYTHON-OR-R

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: PRATEEK MOHAN

*INTERN ID*: CT04DL431

*DOMAIN*: POWER BI

*DURATION*: 4 WEEKS 

*MENTOR*: NEELA SANTOSH

Project: INTEGRATION WITH PYTHON OR R

DATA :- Netflix

Tools & Techniques Used:
Python: matplotlib, seaborn, pandas
Integrating Python and R into Power BI bridges the gap between business intelligence and data science. 
It enables analysts to unlock deeper insights, automate complex analytics, and present results in a user-friendly dashboard format.


# OUTPUT

import matplotlib.pyplot as plt
avg_scores = dataset.groupby('type')['imdb_score'].mean()
avg_scores.plot(kind='bar', color='skyblue')
plt.title('Average IMDb Score by Type')
plt.xlabel('Type')
plt.ylabel('Average IMDb Score')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
![Image](https://github.com/user-attachments/assets/409660c7-85d7-4094-9fa7-0fd06d066c87)


import matplotlib.pyplot as plt
dataset['type'].value_counts().plot(
    kind='pie',
    autopct='%1.1f%%',
    startangle=90,
    figsize=(6, 6),
    ylabel=''
)
plt.title('Distribution of Types')
plt.show()
![Image](https://github.com/user-attachments/assets/9182daaf-41d3-4fce-87e6-d5007dabe912)


import seaborn as sns
import matplotlib.pyplot as plt
sns.countplot(x='imdb_score', data=dataset)
plt.title('IMDb Score')
plt.xlabel('IMDb Score')
plt.ylabel('Frequency')
plt.show()
print(dataset['imdb_score'].value_counts().sort_index())
![Image](https://github.com/user-attachments/assets/6f41cb4f-aa39-4a19-8006-706779717632)


import seaborn as sns
import matplotlib.pyplot as plt

sns.barplot(x='type', y='seasons', data=dataset)
plt.title('Average Number of Seasons by Type')
plt.xlabel('Type')
plt.ylabel('Average Seasons')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
![Image](https://github.com/user-attachments/assets/59457893-4c7b-498c-a91e-0b35c9d333cb)

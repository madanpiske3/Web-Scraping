# Web-Scraping
[Web+Scraping+Cheat+Sheet+2.0.pdf](https://github.com/user-attachments/files/18245540/Web%2BScraping%2BCheat%2BSheet%2B2.0.pdf)

# Cheat Sheet
## Page 1
![cheat-sheet2](https://github.com/user-attachments/assets/dd050eab-5889-4677-b093-f1828fd4582e)

## Page 2
![cheat-sheet1](https://github.com/user-attachments/assets/701b43e4-3d84-4fae-a6fe-3b39e669bdf0)


## Basics of Python for Web Scraping.

###### array index
###### for in
##### if else
##### file
```
with open('filename.txt', 'w') as file:
    file.write('Data successfully scraped!')

# open is a function which takes a file and its type | mode, 
```

##### pandas
pip install pandas

```
import pandas as pd

states = ['Clarifornia', 'Texas', 'Florida', 'New York']
population = [1223224, 34343232, 23335454665, 12345654]

dict_states = {'states': states, 'population': population}
print(dict_states)


df_states = pd.DataFrame.from_dict(dict_states)

print(df_states)

# To convert this into csv
df_states.to_csv('states.csv', index = False)

```

##### Exception Handling
``` py
new_list = [2,4,6, 'India']

for ele in new_list:
    try:
        print(ele / 2)
    except:
        print('The element is not a number')

```

##### While-Break
```
n = 10
while True:
    print(n)
    n-=1
    if n == 1:
        break
print('Loop Exited')

```


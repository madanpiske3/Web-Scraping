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

## HTML for Web Scraping.

### Libraries we need to import

```
pip install bs4
pip install requests
pip install lxml
```
```
Important: Versions of libraries that work for this section
In this section, we'll learn Beautiful Soup. This is the easiest Python library for web scraping, but it has a lot of limitations. This is why we'll learn the essential stuff of web scraping with Beautiful Soup and then move on to more powerful scraping tools.

The scripts work fine with these versions of the libraries (in parentheses the latest versions that also work fine in 2024).


- bs4 4.9.3 (v4.12.3)

- requests 2.25.1

- lxml 4.6.3 (v5.1.0).

You can install a specific version of a library with the command pip install <name-of-library>==<version>


Note: In case you can't install lxml, try installing html.parser (pip install html.parser) and replace lxml with html.parser in the script
```

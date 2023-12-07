
Implémentation technique du meeting optimizer décrit [[README-MO]]

```jupyter
import pandas as pd
import itertools
  

# Define the list of colors
colors = ['rouge', 'jaune', 'vert', 'bleu']

# Generate all possible unique permutations of colors (3 at a time)
permutations = list(itertools.permutations(colors, 3))

# Repeat the permutations to create the DataFrame
df = pd.DataFrame(permutations + permutations, columns=['variable1', 'variable2', 'variable3'])

# Print the DataFrame
print(df)

  
#send the dataframe to a csv file called badges_canope_combinatorics.csv
df.to_csv('badges_canope_combinatorics.csv', index=False)
```

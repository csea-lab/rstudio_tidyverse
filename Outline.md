(The actual code in the talk will be to import data from Matlab and utilize tidyr & dplyr to re-configure for subsequent analysis.)

# Tidyverse 

Tidyverse is a set of packages with code methods to form and to work with rectangular data. Data_frames have variables as columns & cases as rows. Everything else is a matter of getting data into that form.

# Importing data to R

## Readr/Readxl/Haven
- Column specifications define what data type each column of a file will be imported as. 
- By default readr will generate a column spec when a file is read and output a summary. 
- There is a lot to this. So much of data work is getting data to the point where it can be rectanglular.
- When reading in rectangular data, each variable type (as a column) will necessarily be the same type (i.e., always true in SPSS, but never true in Excel).  


# Tidyverse in a nutshell

Tidy data is a way to organize tabular data in a consistent data structure across packages.   

- A table is tidy if:
   - Each variable is in its own column
   - Each observation, or case, is in its own row

# Tidyr

## Tibble (an enhanced r dataframe)
- Tibbles are a table format provided by the tibble package. 
- They inherit the data frame class, but have improved behaviors:
- Subset a new tibble with ], a vector with [[ and $.
- No partial matching when subsetting columns.
- Display concise views of the data on one screen.

## Reshape data

- pivot longer: Pivot data to reorganize values into a new layout.
   - "Lengthen" data by collapsing several columns into two. 
   - Column names move to a new names_to column and values to a new values_to column.

- pivot_wider: inverse of pivot_longer(). 
   - "Widen" data by expanding two columns into several. 
   - One column provides the new column names, the other the values.



read_csv and Matlab (from rmatio - not on cheatsheets)

# Dplyr

## Dplyr - p1:

- pipe data from functions
- manipulate cases (rows)
- manipulate variables (columns)

## Dplyr - p2:

- vectorized functions map 1 to 1 from input to output so number of cases (rows) in =’s number out
- summary functions output less than #of cases in (combined with group_by() from dplyr p.1 determines number of outputs)
- this principle is embodied by the “split-apply-combine” approach 
- relational joins: straight out of linear algebra and  - most of the useful tidyverse meta-programming 



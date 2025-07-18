# VBA Table Manipulation

This project was created to better understand how to use VBA for table manipulation in Excel.

## What it does

- Uses VBA to manage and edit tables  
- Helps practice coding logic directly in Excel

## Why I made it

I built this to improve my VBA skills and learn how to automate table processes for daily tasks.

## How to use

1. Open the Excel file  
2. Enable macros  
3. Check the VBA code to see how each part works

```python
import pandas as pd

file_path = 'CADASTRO_DE_CLIENTE.xlsb'

df = pd.read_excel(file_path, engine='pyxlsb', skiprows=3)

print(df.head())

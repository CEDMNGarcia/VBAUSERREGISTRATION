# Cadastro de Clientes

Esse arquivo é uma planilha com os dados dos clientes, como:

- Nome  
- Celular  
- Data de nascimento  
- CPF  
- Endereço completo (CEP, rua, número, bairro, cidade, estado)  
- Data do cadastro

Também tem alguns campos de controle como ID, ED e EX.

## Sobre o arquivo

- O nome do arquivo é CADASTRO_DE_CLIENTE.xlsb  
- Ele está em formato binário do Excel (.xlsb), mas dá pra abrir normalmente no Excel ou no Python usando pyxlsb.

## Como usar no Python

```python
import pandas as pd

file_path = 'CADASTRO_DE_CLIENTE.xlsb'

df = pd.read_excel(file_path, engine='pyxlsb', skiprows=3)

print(df.head())

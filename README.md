# Desafio 01

Gostaria de Classificar alguns repositórios no github que possuiem releases disponíveis. 

Por Ex.:
```
O repositório: https://github.com/pixies/calculadora-teste-py
Possui ***lançamentos*** (releases), para visualizar siga neste link: https://github.com/pixies/calculadora-teste-py/releases/tag/v1.1
```
Usando o repositório "pixies/calculadora-teste" como exemplo, escreva um programa que consiga identificar e retornar a versão exata do ultimo release disponível.

## Etapa 01

Construir um algoritmo que leia a string: "https://github.com/pixies/devinf/releases/tag/db-base-v1.1" e converte em uma lista.

> REPO: pixies/devinf
> VERSION: db-base-v1.1

***Usem Funções.*** 

```
Ex.:
   nome_completo = "Joao Ferreira de Martins"
   ultimo_nome: ?
   primeiro_nome: ?
 ```

Ideia:
```
def retornar_string_em_lista(string):
    pass

```

## ETAPA 02

Colete o valor da versão do realease de forma automatica direto do site github.com.

Para isso, use a biblioteca ***requests***

```
import requests

requisicao = requests.get('https://github.com/usario/repositorio/releases/latest')
print(requisicao.url)
```
***Usem Funções***


## Etapa 03

Salvar os dados coletados.

> REPO: pixies/devinf
> VERSION: db-base-v1.1

### Salvar em DataFile

***Fonção Open***
Observações:
```
Arquivos tem modos: 
  - Ler (read) - r (read, realine, readlines)
  - Escrever (writer) - w (write) - crio
  - Adicionar (append) - a (write) - adicionando dados
  - Binario (bin) - b 

***Ler arquivo***
> arquivo_01 = open('arquivo.txt', 'r') # retornar error

***Cria novo arquivo***
> arquivo_02 = open('arquivo02.txt', 'w')

***Ler arquivo***
> arquivo_01 = open('arquivo.txt', 'r')
```
1. Criem funcoes para criar arquivos.
2. Abra o arquivo "usando a flag 'a'" para salvar no datafile os dados:
{'REPO':'pixies/devinf','VERSION':'db-base-v1.1'}

### Resumo:

1. ETAPA 01 E 02 (Coletar os dados da versao do release desejado)
2. SALVAR OS DADOS EM UM DATAFILE


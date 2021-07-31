# Exercício prático de Banco de Dados | Mongo db


Projeto Prático com Banco de Dados e Mongo db

Descrição do Projeto: 
Você deve criar um banco de dados novo (database) e uma coleção com um nome pertinente, de acordo com os dados e tema que você escolher. Os seguintes comandos devem ser feitos e entregues:

Inserção de documentos
Atualização de documentos
Exclusão de documentos
Consulta com projeção
Consulta utilizando combinação entre os seletores
Consulta paginada e ordenada (utilizar skip, limit e sort)

Comandos utilizados na resolução das demandas:
Inicializei o mongo db através do terminal windows (Prompt de Comando) e iniciei a conexão com o Robot 3t, através da porta Reprograma, criada na aula do dia 23/07/2021

##Inserção de documentos na collection
Criei um arquivo json de filmes que gosto e inclui na collection que nomei de "filmes"

db.filmes.insertMany([
    {
    
        "nome": "",
        "genero": "",
        "classificacao": "",
        "tempo de duracao": "",
        "ano": ""
    },

{        "nome": "",
        "genero": "",
        "classificacao": "",
        "tempo de duracao": "",
        "ano": ""
    },

{
        "nome": "",
        "genero": "",
        "classificacao": "",
        "tempo de duracao": "",
        "ano": ""
    },
{
        "nome": "",
        "genero": "",
        "classificacao": "",
        "tempo de duracao": "",
        "ano": ""
    }
    ])
    
##Atualização de documentos

db.getCollection('filmes').update(
    {
        "Nome": ""
    },
    
    {
        $set:{"Ano" : ""}
    }
  )

##Exclusão de documentos
db.filmes.remove({"Ano": ""})

##Consulta com projeção
Filmes ordenados do ano mais recente ao mais antigo.

db.getCollection("filmes").find().sort({"Ano": -1})
Filmes ordenados do ano mais antigo ao mais recente.

db.getCollection("filmes").find().sort({"Ano": 1})
Consulta utilizando combinação entre os seletores
db.getCollection("filmes").find({"Genero":"","Ano":""})
Consulta paginada e ordenada
Consulta pela classificação, limitando a dois filmes.

db.getCollection("filmes").find({"Classificação": ""}).limit(2)

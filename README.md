# AfBancoDeDadosNoSQL
Continuação da atividade final realizando agora as etapas 1, 2 e 3 em NoSQL

## Etapa 1: 
Um usuário configura seu navegador com os seguintes dados:

página inicial: www.google.com

Idioma preferido: Português do Brasil

Localização: São Paulo

Tema: Clássico

Mostrar favoritos: Sim

Zoom: 100%

Escreva os dados acima na notação JSON. Para esta atividade utilize o bloco de notas, salve o arquivo com o nome: localização_google_sp.json

![image](https://github.com/CaioHessel/AfBancoDeDadosNoSQL/assets/64332918/c1336078-1c40-4f15-8628-0548a481f530)


## Etapa 2:

Crie, conforme o modelo relacional, as tabelas normalizadas. Crie também um documento JSON que contenha esses dados.

### 1FN
Aplicando a primeira forma normal a tabela usada no exemplo precisamos eliminar os atributos multivalorados em cada linha, que no caso são e-mail e endereço.

![image](https://github.com/CaioHessel/AfBancoDeDadosNoSQL/assets/64332918/836b0927-50a4-498c-acd5-4f3f4a699154)

### 2FN

Aplicando a segunda forma normal precisamos ajustar as dependências, sendo que cada coluna não chave deve fazer referência a chave primária completa. Sendo assim a coluna e-mail passa a ser uma nova tabela tendo como referência os nomes.

![image](https://github.com/CaioHessel/AfBancoDeDadosNoSQL/assets/64332918/64498cba-1d8c-4882-9a58-dd68373664a0)

### 3FN

Para a Terceira Forma Normal, precisamos eliminar dependências transitivas. Isso significa que qualquer coluna não chave deve depender apenas da chave primária, e não de outras colunas não chave. Na tabela Funcionários, podemos notar que Salário pode depender de Cargo, então precisamos separar isso para garantir que não haja dependências transitivas.

![image](https://github.com/CaioHessel/AfBancoDeDadosNoSQL/assets/64332918/61f05b0a-8a2a-4b63-a59a-0e5ed4d6f7b2)

### Etapa 3

Crie um banco de dados NoSQL no Firebase conforme foi demonstrado no conteúdo da aula sobre banco de dados não relacionais;
Ao término do exemplo, crie um segundo banco de dados, mas utilizando o tema Jogos;
Nesse banco deve haver, coleções de personagens, jogos e fabricante.

![image](https://github.com/CaioHessel/AfBancoDeDadosNoSQL/assets/64332918/db24b425-b3df-4636-85db-1c11a92482d8)

Aluno: Caio Cesar Hessel de Oliveira
Ra: 200357

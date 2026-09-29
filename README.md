site-soma

Projeto desenvolvido como exercício da disciplina, com o objetivo de praticar o uso do Express (framework do Node.js) para criar um servidor com rotas GET e POST.

O que o projeto faz

O servidor expõe uma rota GET /, que retorna uma mensagem simples de boas-vindas, e quatro rotas POST que recebem dois números (a e b) no corpo da requisição (em formato JSON) e retornam o resultado de uma operação matemática:

POST /soma → retorna a soma de a e b
POST /subtracao → retorna a subtração de a e b
POST /multiplicacao → retorna a multiplicação de a e b
POST /divisao → retorna a divisão de a e b
Tecnologias utilizadas
Node.js — ambiente de execução do JavaScript fora do navegador
Express — framework para criação do servidor e das rotas
body-parser — biblioteca usada para interpretar o corpo (body) das requisições em formato JSON
Como rodar o projeto
Clone este repositório ou baixe os arquivos.
No terminal, dentro da pasta do projeto, instale as dependências:
   npm install
Inicie o servidor:
   node app.js
O servidor ficará disponível em http://localhost:3001.
Como testar
GET: acesse http://localhost:3001/ pelo navegador.
POST: use o Postman, enviando uma requisição POST para as rotas acima (ex: http://localhost:3001/soma), com um corpo em JSON, por exemplo:
json
  {
    "a": 10,
    "b": 5
  }
Evidências de funcionamento

GET - Acesso à rota inicial:

<img width="1887" height="1010" alt="servidor node" src="https://github.com/user-attachments/assets/02ab0360-b2ee-4a62-997a-2e7ad07f1b47" />

POST - Rota /soma:

<img width="1900" height="1062" alt="soma" src="https://github.com/user-attachments/assets/a190b49b-166a-4793-8460-be9cb4eae190" />


POST - Rota /subtracao

<img width="1917" height="1078" alt="subtração" src="https://github.com/user-attachments/assets/f8c7ccda-683a-45b2-b6fb-f2f24d7b2a33" />


POST - Rota /multiplicacao

<img width="1917" height="1078" alt="multiplicação" src="https://github.com/user-attachments/assets/93fa9e79-1aa4-4708-a8a3-9a02eac3e2d4" />


POST - Rota /divisao

<img width="1917" height="1078" alt="divisão" src="https://github.com/user-attachments/assets/5694266c-2cb5-44d3-99e1-ed21944d432b" />

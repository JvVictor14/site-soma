# site-soma

Exercício Express: servidor com rotas POST para soma, subtração, multiplicação e divisão.

## Como rodar

1. Extraia os arquivos em uma pasta chamada `site-soma`.
2. Abra a pasta no VS Code.
3. No terminal, instale as dependências:
   ```
   npm install
   ```
4. Inicie o servidor:
   ```
   node app.js
   ```
5. Acesse no navegador: http://localhost:3001/ (deve mostrar "Oi, mundo :-)")

## Testando no Postman

Para cada operação, crie uma requisição:

- **Método:** POST
- **URL:** `http://localhost:3001/soma` (ou `/subtracao`, `/multiplicacao`, `/divisao`)
- **Body:** selecione `raw` e `JSON`, e envie algo como:
  ```json
  {
    "a": 10,
    "b": 5
  }
  ```

### Exemplos de rotas disponíveis

| Rota              | Operação       |
|-------------------|----------------|
| POST /soma         | a + b          |
| POST /subtracao     | a - b          |
| POST /multiplicacao | a * b          |
| POST /divisao       | a / b          |

O resultado vem como texto na resposta, por exemplo:
```
O resultado da soma de 10 e 5 é 15
```

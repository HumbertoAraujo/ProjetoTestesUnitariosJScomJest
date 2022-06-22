# Requisitos Obrigatórios

⚠️ Lembre-se de que o seu projeto só será avaliado se estiver passando por **todos os _checks_** do **Linter**. Utilize o comando `npm run lint` no seu terminal para verificar os _checks_ do **Linter** 😉 ⚠️

---

### 1. Implemente a função `average`

<details>
  <summary>A função average recebe um array de tamanho variável e retorna a média dos valores recebidos. Caso a função receba algum valor não numérico ou um array vazio, o valor `undefined` deve ser retornado.</summary><br/> 
  
  Todos os resultados devem ser arredondados para valores inteiros. Ex: 4,6 vira 5; 1,3 vira 1. O arquivo `average.spec.js` contém os testes para `average` já implementados. Implemente a função no arquivo `src/average.js` de forma que ela atenda aos testes propostos.

  **O que será testado:**

  - Será validado se, ao receber um array de números, a função `average` retorna a média de seus valores;
  - Será validado se, ao receber um array que contém valores não numéricos, a função `average` retorna `undefined`;
  - Será validado se, ao receber um array vazio, a função `average` retorna `undefined`.

</details>

---

### 2. Implemente os casos de teste para a função `numbers`

<details>
  <summary>A função `numbers` recebe um array de tamanho variável e retorna `true` se todos os parâmetros forem do tipo 'number' e `false` caso contrário.</summary><br/> 
  
  Essa função já está implementada no arquivo `src/numbers.js`. Escreva pelo menos quatro testes para essa função para garantir que a implementação de `numbers` está correta.

  **O que será testado:**

  - Será validado se no teste da função `numbers`, o retorno da função é `true` quando o array passado por parâmetro contém somente números.

</details>

---

### 3. Implemente a função `vqv`

<details>
  <summary>Use template literals para escrever uma função que recebe o seu nome e a sua idade e retorna o parágrafo descrito abaixo:</summary><br/>

  ```javascript
  `Oi, meu nome é Tunico!
  Tenho 30 anos,
  trabalho na Trybe e mando muito em programação!
  #VQV!`
  ```

  Caso a função seja chamada sem nenhum parâmetro, o valor `undefined` deve ser retornado. O arquivo `vqv.spec.js` contém os testes para `vqv` já implementados. Implemente a função no arquivo `src/vqv.js` de forma que ela atenda aos testes propostos.

  **O que será avaliado**

  - Será validado se `vqv` é uma função;
  - Será validado se a função `vqv` retorna dados do tipo string;
  - Será validado se a função `vqv` retorna a frase esperada quando passados parâmetros de nome e idade;
  - Será validado se a função `vqv`, quando chamada sem parâmetro, retorna `undefined`.

</details>

---

### 4. Implemente os casos de teste para a função `circle`

<details>

  <summary>A função `circle` recebe o raio de um círculo e retorna um objeto contendo as suas informações: Raio, Área e Circunferência. Se não for especificado um raio, a função retorna `undefined`.</summary></br>
  
  Essa função já está implementada no arquivo `src/circle.js`. Escreva pelo menos seis testes para essa função para garantir que a implementação de `circle` está correta.

  **O que será avaliado**

  - Será validado se no teste da função `circle`, ao receber um raio, o retorno da função é um objeto com as informações corretas (Raio, Área e Circunferência).

</details>

---

### 5. Implemente a função `createStudent`

<details>
<summary>A função `createStudent` recebe como parâmetro um **nome**, e retorna um objeto contendo duas chaves:</summary></br>

  1. **name**, contendo o nome passado como parâmetro;
  2. **feedback**, contendo uma função que retorna a frase 'Eita pessoa boa!' ao ser chamada.

  O arquivo `createStudent.spec.js` contém os testes para `createStudent` já implementados. Implemente a função no arquivo `src/createStudent.js` de forma que ela atenda aos testes propostos.

  **O que será avaliado**

  - Será validado se a função `createStudent` retorna um objeto que contenha duas chaves: `name`, contendo o nome passado como parâmetro; e `feedback`, contendo uma função que retorna a frase 'Eita pessoa boa!' ao ser chamada.

</details>

---

### 6. Implemente os casos de teste para a função `productDetails`

<details>
  <summary>A função `productDetails` recebe duas strings que representam nomes de produtos, e retorna um array contendo dois objetos com os detalhes dos respectivos produtos:</summary></br>

  ```javascript
  productDetails('Alcool gel', 'Máscara');
  ```

  **Retorna:**

  ```js
  [
    {
      name: 'Alcool gel'
      details: {
        productId: 'Alcool gel123'
      }
    },
    {
      name: 'Máscara'
      details: {
        productId: 'Máscara123'
      }
    }
  ]
  ```

  Essa função já está implementada no arquivo `src/productDetails.js`. Escreva pelo menos cinco testes para essa função no arquivo `tests/productDetails.js` para garantir que a implementação de `productDetails` está correta.

  **O que será avaliado**

  - Será validado se no teste da função `productDetails`, ao receber duas strings, o retorno da função é um array de objetos e se cada objeto contém os dados necessários.

</details>

---

### 7. Implemente as funções `calculator` e `arrayGenerator`

<details>
  <summary>A função `calculator` recebe dois números inteiros como parâmetro e retorna um objeto com as seguintes chaves:</summary></br>
  - sum;
  - mult;
  - div;
  - sub.

  Para cada chave atribua como valor a operação correspondente à sua chave:
  - `sum:` retorna o resultado da soma dos dois números;
  - `mult:` retorna o resultado da multiplicação dos dois números;
  - `div:` retorna o resultado da divisão dos dois números;
  - `sub:` retorna o resultado da subtração dos dois números.

  Os resultados das divisões devem sempre ser arredondados para baixo.

  Parâmetros:
  - Dois números inteiros.

  Comportamento:
  ```javascript
  calculator(1, 2); // { sum: 3, mult: 2, div: 0, sub: -1 }
  ```

  Já a função `arrayGenerator` converte objetos em arrays, de chaves, valores ou ambos. Ela deve receber dois parâmetros:

  - o primeiro parâmetro deve ser uma string que indica o tipo de conversão;
  - o segundo parâmetro deve ser um objeto semelhante ao que é retornado pela função calculator que você acabou de desenvolver.

  Parâmetros:
  - Uma string que indica o tipo de conversão;
  - Um objeto no formato { sum: 3, mult: 2, div: 0, sub: -1 };

  Comportamento:
  ```javascript
  arrayGenerator('keys', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 'sum', 'mult', 'div', 'sub' ]
  arrayGenerator('values', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ 3, 2, 1, 0 ]
  arrayGenerator('entries', { sum: 3, mult: 2, div: 1, sub: 0 }) // [ [ 'sum', 3 ], [ 'mult', 2 ], [ 'div', 1 ], [ 'sub', 0 ] ]
  ```
  O arquivo `objPlayground.spec.js` contém os testes para `calculator` e `arrayGenerator` já implementados. Implemente as funções no arquivo `src/objPlayground.js` de forma que ela atenda aos testes propostos.

  **O que será avaliado**

  - Será avaliado se a função `calculator` retorna os valores esperados;
  - Será avaliado se a função `arrayGenerator` retorna os valores esperados.

</details>

---

### 8. Implemente a função `myCounter`

<details>
  <summary>A função myCounter possui dois loops aninhados que inserem valores dentro de um array. Como podemos perceber, eles vão adicionando valores ao array até sua condição de parada.</summary></br>

   Corrija a função `myCounter`, sem eliminar nenhum dos loops de repetição, para que a função retorne o array correto. O arquivo `myCounter.spec.js` contém os testes para `myCounter` já implementados. Implemente a função no arquivo `src/myCounter.js` de forma que ela atenda aos testes propostos.

  **O que será avaliado**

  - Será validado se a função `myCounter` retorna os dados esperados de acordo com o que está implementado no teste.

</details>

---

### 9. Implemente os casos de teste para a função `getCharacter`

<details>

  <summary>A função `getCharacter` recebe uma string que representa o nome de uma personagem e retorna um objeto contendo o seu nome, a sua classe e as suas frases.</summary></br>

  ```javascript
  getCharacter('Arya');
  ```

  **Retorna:**

  ```javascript
  {
    name: 'Arya Stark',
    class: 'Rogue',
    phrases: ['Not today', 'A girl has no name.']
  }
  ```

  Essa função já está implementada no arquivo `src/getCharacter.js`. Escreva pelo menos seis testes para essa função no arquivo `tests/getCharacter.spec.js` para garantir que a implementação de `getCharacter` está correta.

  **O que será avaliado**

  - Será validado se no teste da função `getCharacter` ao receber uma string, o retorno da função é o esperado - de acordo com a tabela apresentada no arquivo de testes.
  - Será validado se no teste da função `getCharacter` ao não receber nenhum parâmetro, o retorno da função é `undefined`.
  - Será validado se o teste da função `getCharacter` verifica se o parâmetro é case sensitive.

</details>

---

### 10. Implemente a função `createMenu`, bem como seus casos de teste

<details>
  <summary>Esse último requisito vai guiar você por um rico processo de Desenvolvimento Orientado a Testes ou TDD - Test Driven Development</summary></br>

  Imagine a seguinte situação: você é responsável por escrever o código do sistema de pedidos de um restaurante através do qual será possível cadastrar um menu. Dado que um menu foi cadastrado, o sistema deve disponibilizar um objeto que permite:

  - Ler o menu cadastrado;
  - Fazer pedidos;
  - Verificar o que foi pedido;
  - Somar o valor da conta.

  A estrutura deste código e deste objeto já está definida e você precisa implementá-la. Você encontrará mais detalhes sobre a estrutura a ser seguida e exemplos do retorno da função no arquivo `src/restaurant.js`. 
  Você deverá se orientar através dos tópicos abaixo para garantir o bom desenvolvimento do sistema.

  **IMPORTANTE - BOAS PRÁTICAS TDD: COMECE PELO TESTE 1 DO ARQUIVO `tests/restaurant.spec.js`** 
</details>

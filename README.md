# Calculadora de Equação de Segundo Grau

Projeto de uma aplicação web para calcular as raízes de uma equação de segundo grau utilizando a fórmula de Bhaskara.

A aplicação permite informar os valores de `a`, `b` e `c`, calcular o valor de Delta e, a partir dele, identificar e apresentar as raízes reais da equação.

## Sobre o projeto

Uma equação de segundo grau possui o formato:

```text
ax² + bx + c = 0
```

Para encontrar suas raízes, o projeto utiliza a fórmula de Bhaskara.

Primeiro, é calculado o valor de Delta:

```text
Δ = b² - 4ac
```

Depois, quando existem raízes reais, são calculados os valores de `x₁` e `x₂`:

```text
x = (-b ± √Δ) / 2a
```

## Funcionalidades

* Informar os valores de `a`, `b` e `c`.
* Calcular o valor de Delta.
* Calcular duas raízes reais quando Delta é maior que zero.
* Identificar quando a equação possui apenas uma raiz real quando Delta é igual a zero.
* Informar quando não existem raízes reais quando Delta é menor que zero.
* Validar se os valores informados são numéricos.
* Verificar se o valor de `a` é diferente de zero.
* Limpar os campos e o resultado do cálculo.

## Tecnologias utilizadas

* HTML5
* CSS3
* JavaScript

## Estrutura do projeto

```text
Calculando_Bhaskara-master/
│
├── index.html
│
├── css/
│   └── style.css
│
├── js/
│   └── script.js
│
└── img/
    └── logo.png
```

## Arquivos

### index.html

Responsável pela estrutura da aplicação.

O arquivo contém:

* Explicação sobre a equação de segundo grau.
* Fórmula de Bhaskara.
* Campos para inserir os valores de `a`, `b` e `c`.
* Botão para realizar o cálculo.
* Botão para limpar os dados.
* Área para apresentar o resultado.

### css/style.css

Responsável pela aparência da aplicação.

O CSS define:

* Cores da página.
* Tipografia.
* Espaçamentos.
* Formatação dos campos.
* Estilização dos botões.
* Área de resultado.
* Cartão principal da calculadora.
* Layout responsivo.

### js/script.js

Responsável pela lógica da aplicação.

A função `calcularBhaskara()`:

1. Obtém os valores de `a`, `b` e `c`.
2. Verifica se os valores são válidos.
3. Verifica se `a` é diferente de zero.
4. Calcula o Delta.
5. Verifica o resultado de Delta.
6. Calcula e apresenta as raízes quando existirem.

A função `fLimpar()` remove os valores inseridos nos campos e restaura a mensagem inicial da área de resultado.

## Tratamento de Delta

O sistema considera três situações:

### Delta maior que zero

A equação possui duas raízes reais diferentes.

```text
x₁ = (-b + √Δ) / 2a

x₂ = (-b - √Δ) / 2a
```

### Delta igual a zero

A equação possui uma única raiz real.

```text
x = -b / 2a
```

### Delta menor que zero

A equação não possui raízes reais.

## Validações

O sistema possui algumas validações para evitar cálculos inválidos.

Caso algum dos valores não seja informado corretamente, uma mensagem é apresentada solicitando os valores de `a`, `b` e `c`.

Também é verificado se `a` é diferente de zero, pois uma equação de segundo grau precisa possuir um coeficiente `a` diferente de zero.

## Como executar

1. Faça o download ou clone o repositório.
2. Abra a pasta `Calculando_Bhaskara-master`.
3. Abra o arquivo `index.html` em um navegador.
4. Informe os valores de `a`, `b` e `c`.
5. Clique em **Calcular**.
6. O resultado será apresentado na área abaixo do formulário.

Não é necessário instalar dependências ou utilizar um servidor para executar o projeto.

## Objetivo

O projeto foi desenvolvido para praticar conceitos fundamentais de desenvolvimento web e lógica de programação, utilizando JavaScript para implementar os cálculos matemáticos e HTML e CSS para criar a interface da aplicação.

## Autor

Mylena Dantas Guimarães

# SPTecher's Machine - Sistema de Numeração

## Descrição

O **SPTecher's Machine** é uma calculadora de conversão entre diferentes bases numéricas, incluindo **Binário (Base 2)**, **Decimal (Base 10)**, **Octal (Base 8)** e **Hexadecimal (Base 16)**. O sistema permite que você converta rapidamente números entre essas bases, facilitando o estudo e aplicação de sistemas numéricos em várias áreas, como computação, programação e matemática.

## Funcionalidades

- **Conversão entre bases numéricas**: Suporta conversões entre os sistemas **Binário**, **Decimal**, **Octal** e **Hexadecimal**.
- **Interface simples e fácil de usar**: A entrada e visualização do resultado são rápidas e diretas.
- **Conversão automática**: Após inserir um número e escolher sua base, o sistema converte o valor para todas as outras bases e exibe os resultados.

## Como Usar

1. **Escolha a base numérica** de entrada (Binário, Decimal, Octal ou Hexadecimal) através de um menu suspenso.
2. **Digite o valor** no campo de entrada correspondente à base selecionada.
3. **Clique em "Calcular"** para converter o número para as outras bases.
4. **Visualize o resultado** nas bases **Binária**, **Decimal**, **Octal** e **Hexadecimal**.

## Lógica do Código JavaScript

A função principal do JavaScript é a `calcular()`, que manipula as entradas do usuário e realiza as conversões entre bases. O fluxo de funcionamento é o seguinte:

1. **Obtenção dos valores de entrada**: A função pega o valor digitado pelo usuário e a base numérica selecionada.
2. **Verificação da base selecionada**: Dependendo da base escolhida (Binário, Decimal, Octal ou Hexadecimal), a função aplica uma lógica específica para validar e converter o valor inserido para Decimal.
3. **Conversão para Decimal**: Para cada base, o valor é convertido para o formato decimal, que é a base comum para todas as conversões.
4. **Conversões para outras bases**: Após obter o valor em Decimal, a função converte esse número para Binário, Octal e Hexadecimal, e exibe os resultados.

Exemplo de como a conversão é feita para a base Binária:

```javascript
while (tamanho > 0) {
    var digito = valor[tamanho - 1];
    valorEmDecimal += digito * (2 ** potencia); // Converte para Decimal
    tamanho--;
    potencia++;
}

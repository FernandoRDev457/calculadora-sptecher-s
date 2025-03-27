# SPTecher's Machine - Sistema de Numeração

## ✨ Descrição

O **SPTecher's Machine** é uma calculadora de conversão entre diferentes bases numéricas, incluindo **Binário (Base 2)**, **Decimal (Base 10)**, **Octal (Base 8)** e **Hexadecimal (Base 16)**. Este sistema é perfeito para quem deseja realizar conversões rápidas entre as bases numéricas mais comuns no mundo da programação, computação e matemática.

Com a **SPTecher's Machine**, você pode:
- Converter entre diferentes bases numéricas sem complicação.
- Explorar como diferentes sistemas de numeração funcionam.
- Aprender sobre a importância das bases numéricas no mundo da computação.

## 🛠️ Funcionalidades

- **Conversão entre Bases Numéricas**: Realize conversões entre **Binário**, **Decimal**, **Octal** e **Hexadecimal** de maneira simples e intuitiva.
- **Interface Simples e Interativa**: A interface é fácil de usar, permitindo uma conversão rápida sem complicação.
- **Resultados Instantâneos**: Após inserir o número e escolher a base, os resultados são calculados e exibidos em todas as outras bases automaticamente.

## 🚀 Como Usar

1. **Escolha a Base Numérica** de entrada (Binário, Decimal, Octal ou Hexadecimal).
2. **Digite o Valor** no campo de entrada correspondente à base selecionada.
3. **Clique em "Calcular"** para realizar a conversão.
4. **Visualize os Resultados** nas bases **Binária**, **Decimal**, **Octal** e **Hexadecimal**.

## 🧑‍💻 Lógica do Código JavaScript

A função `calcular()` é o coração do código, realizando as conversões entre bases. Aqui está como ela funciona:

1. **Obtenção de Dados**: Pega o valor inserido pelo usuário e a base selecionada.
2. **Verificação da Base**: Verifica qual base foi selecionada (Binário, Decimal, Octal ou Hexadecimal) e executa a lógica de conversão apropriada.
3. **Conversão para Decimal**: Independente da base de entrada, o valor é convertido para **Decimal**, que é a base intermediária para as conversões.
4. **Conversões para Outras Bases**: A partir do valor em Decimal, o número é então convertido para Binário, Octal e Hexadecimal.

### Exemplo de Conversão para Binário:
```javascript
while (tamanho > 0) {
    var digito = valor[tamanho - 1]; 
    valorEmDecimal += digito * (2 ** potencia); // Converte para Decimal
    tamanho--; 
    potencia++;
}

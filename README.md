# 🧮 **Calculadora Simples em Java (sem `if/else`)!**
Este é um exercício de uma calculadora em Java que realiza operações básicas **sem utilizar estruturas `if/else`**, apenas com **operadores ternários (`? :`)**.
## **Funcionalidades Suportadas**
- **`+` Soma**  
- **`-` Subtração**  
- **`*` Multiplicação**  
- **`/` Divisão**  
- **`%` Módulo** (resto da divisão)
## **Exemplo de Uso**
O usuário deve fornecer:
1. Primeiro número  
2. Segundo número  
3. Operação desejada (`+`, `-`, `*`, `/`, `%`)
**Exemplo de entrada/saída:**
```
Informe o número: 10
Informe o número: 2
Informe a operação: *
10.00 * 2.00 = 20.00
```
## **Lógica (sem `if/else`)**
A operação é determinada por uma **cadeia de operadores ternários**:
```java
double resultado = "+".equals(op) ? num1 + num2 : 0;
resultado = "-".equals(op) ? num1 - num2 : resultado;
resultado = "*".equals(op) ? num1 * num2 : resultado;
resultado = "/".equals(op) ? num1 / num2 : resultado;
resultado = "%".equals(op) ? num1 % num2 : resultado;
```
### Explicação:
- Cada linha verifica **uma operação** específica.
- Se a condição for verdadeira, calcula o resultado correspondente.
- Se falsa, mantém o valor anterior de `resultado`.
- A última operação verificada define o resultado final.
## **Observações Importantes**
- **Não valida** se a operação informada é válida (caso digite um operador inválido, o resultado será 0 ou o último cálculo válido).
- **Não trata divisão por zero** (se dividir por zero, ocorrerá um erro).
- **Propósito didático**: este código é um exercício para entender operadores ternários.
> Requer implementação de validações para uso real.

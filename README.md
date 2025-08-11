
# 📌 Analisador Léxico para Linguagem P

Este projeto implementa um **analisador léxico** simples para a linguagem fictícia **P**, capaz de identificar palavras-chave, símbolos, números e identificadores presentes em um código-fonte.

---

## 🚀 Funcionalidades

✅ Reconhece **palavras-chave** da linguagem P  
✅ Identifica **símbolos** e operadores (matemáticos, lógicos e de comparação)  
✅ Classifica **números** (inteiros e reais)  
✅ Reconhece **identificadores** (variáveis, nomes de funções, etc.)  
✅ Imprime o tipo de cada token encontrado  

---

## 🗂 Estrutura do Código

O código é dividido em três partes principais:

1. **Definição de palavras-chave e símbolos**  
   - `keywords`: lista com todas as palavras-chave da linguagem P.  
   - `symbols`: dicionário que mapeia operadores e símbolos para suas descrições.

2. **Funções auxiliares**  
   - `is_number(token)`: verifica se o token é um número (inteiro ou real).  
   - `lexer(input_code)`: função principal que divide o código em tokens e classifica cada um.

3. **Execução de exemplo**  
   - Um código fictício em P é utilizado para demonstrar o funcionamento do analisador.

---

## 📄 Exemplo de Código em P

```p
inteiro x = 10;
real y = 20.5;
se (x > y) {
    mostrar(x);
} senao {
    ler(y);
}

---

Saída Esperada

Palavra-chave: inteiro
Identificador: x
Operador de atribuição: =
Identificador: 10;
Palavra-chave: real
Identificador: y
Operador de atribuição: =
Identificador: 20.5;
Palavra-chave: se
Identificador: (x
Operador maior que: >
Identificador: y)
Inicia bloco de comandos: {
Identificador: mostrar(x);
Fecha bloco de comandos: }
Palavra-chave: senao
Inicia bloco de comandos: {
Identificador: ler(y);
Fecha bloco de comandos: }




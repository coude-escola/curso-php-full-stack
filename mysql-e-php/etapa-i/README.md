## **🎯 Objetivos da Etapa**

- **PHP (parte 1) - tipos de valores, variáveis e constantes**
- **PHP (parte 2) - operadores**
- **PHP (parte 3) - condicionais: if e else, ternários, switch**

---

## **🛠️ 1. PHP (parte 1) - Tipos de Valores, Variáveis e Constantes**

No PHP, os tipos de valores, variáveis e constantes são a base para qualquer aplicação funcional. Entender como cada um funciona é essencial para manipular dados de forma eficiente.

### **📚 Tipos de Valores:**

Os principais tipos de valores no PHP incluem:

- **null:** Representa uma variável sem valor.
- **bool:** Valores booleanos, ou **lógicos** (`true` ou `false`).
- **string:** Cadeias de texto.
- **int:** Números inteiros.
- **float:** Números decimais.
- **array:** Conjunto de valores.
- **object:** Representação de objetos.

**💡 Exemplo Analógico:** Pense nos tipos de valores como diferentes recipientes de cozinha. Cada recipiente (tipo de dado) é adequado para armazenar um tipo específico de alimento (valor). Uma string é como um pote de vidro para armazenar palavras, enquanto um array é como uma caixa organizadora com várias divisórias para diferentes elementos.

### **🔑 Variáveis e Constantes:**

- **Variáveis:** Armazenam valores temporários e podem ser alteradas durante a execução do programa.
- **Constantes:** Armazenam valores fixos que não podem ser alterados durante a execução do programa.

**Exemplo Prático:**

```php
$nome = "COUDE"; // Variável
const VERSAO = "1.0.0"; // Constante
define("EMPRESA", "COUDE Escola de Tecnologia"); // Constante usando define
```

---

## **💻 2. PHP (parte 2) - Operadores**

Os operadores permitem realizar operações entre valores e variáveis. Eles são fundamentais para processar informações e definir regras de lógica.

### **🔄 Tipos de Operadores:**

- **Aritméticos:** `+`, `-`, `*`, `/`, `%`
- **Comparação:** `==`, `!=`, `>`, `<`, `>=`, `<=`
- **Lógicos:** `&&`, `||`, `!`
- **Atribuição:** `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `**=`, \`.=\`\`

**💡 Exemplo Analógico:**
Os operadores funcionam como ferramentas em uma caixa de ferramentas. O operador de adição (`+`) é como um martelo que junta peças, enquanto o operador de comparação (`==`) é como uma régua que mede se duas peças têm o mesmo tamanho.

**Exemplo Prático:**

```php
$a = 5;
$b = 10;
$resultado = $a + $b; // Soma
$igual = ($a == $b); // Comparação
$a += 2; // Atribuição: $a agora é 7
$b *= 3; // Atribuição: $b agora é 30
```

### **🔗 Concatenação de Strings:**

No PHP, podemos unir (concatenar) strings utilizando o operador `.`.

**Exemplo Prático:**

```php
$nome = "COUDE";
$versao = "1.0.0";
$mensagem = "Bem-vindo à " . $nome . " versão " . $versao;
echo $mensagem;
// Saída: Bem-vindo à COUDE versão 1.0.0
```

**💡 Exemplo Analógico:**
Concatenar strings é como juntar peças de um quebra-cabeça. Cada string é uma peça, e o operador `.` é a cola que as une para formar uma mensagem completa.

---

## **🌍 3. PHP (parte 3) - Condicionais: if, else, else if, ternários, switch**

As estruturas condicionais permitem que o código tome decisões com base em condições específicas.

### **🧠 Tipos de Estruturas Condicionais:**

- **if:** Executa um bloco de código se a condição for verdadeira.
- **else:** Executa um bloco alternativo se a condição for falsa.
- **else if:** Permite verificar múltiplas condições em sequência.
- **ternário:** Uma forma simplificada de if-else.
- **switch:** Permite verificar várias condições de uma vez.

**💡 Exemplo Analógico:**

- **if-else:** Como um portão com duas saídas, onde você pode ir para um lado ou para outro.
- **else if:** Como uma série de semáforos, onde cada condição é verificada em sequência.
- **ternário:** Como um atalho para uma decisão rápida.
- **switch:** Como um painel de botões, onde cada botão representa um caso específico.

**Exemplo Prático:**

```php
$nota = 85;
if ($nota >= 90) {
    echo "Aprovado com excelência";
} else if ($nota >= 70) {
    echo "Aprovado";
} else {
    echo "Reprovado";
}

$idade = 18;
echo ($idade >= 18) ? "Maior de idade" : "Menor de idade";

$opcao = 2;
switch ($opcao) {
    case 1:
        echo "Opção 1 selecionada";
        break;
    case 2:
        echo "Opção 2 selecionada";
        break;
    default:
        echo "Opção inválida";
}
```

---

**📝 4. Proposta de Exercícios**

### **✅ Exercício 1:**

- **🎯 Objetivo:** Compreender tipos de dados.
- **📝 Instrução:** Crie variáveis com cada tipo de dado abordado (`null`, `bool`, `string`, `int`, `float`, `array`, `object`) e exiba seus valores usando `echo`.

### **✅ Exercício 2:**

- **🎯 Objetivo:** Praticar operadores.
- **📝 Instrução:** Desenvolva um programa PHP que receba dois números e realize as operações aritméticas básicas (`+`, `-`, `*`, `/`, `%`). Exiba os resultados.

### **✅ Exercício 3:**

- **🎯 Objetivo:** Usar estruturas condicionais.
- **📝 Instrução:** Crie um sistema que receba a nota de um aluno e exiba a classificação (`Aprovado com excelência`, `Aprovado`, `Reprovado`) utilizando `if`, `else if` e `else`. Em seguida, converta a lógica para um operador ternário.

### **✅ Exercício 4:**

- **🎯 Objetivo:** Explorar switch.
- **📝 Instrução:** Crie um sistema que exiba o dia da semana com base em um número fornecido pelo usuário (`1` para segunda-feira, `2` para terça-feira, etc.) usando `switch`.


## **🎯 Objetivos da Etapa**

- **HTML (parte 3) - Formulários**
- **Métodos GET e POST - como utilizar**
- **PHP (parte 9) - SESSION**

---

## **🛠️ 1. HTML (parte 3) - Formulários**

Os formulários HTML são fundamentais para capturar dados de usuários e enviá-los para o servidor para processamento.

### **📚 Estrutura de um Formulário HTML:**

- **form:** Define o início e o fim do formulário.
- **action:** Define para onde os dados serão enviados.
- **method:** Especifica como os dados serão enviados (`GET` ou `POST`).
- **input:** Campos para entrada de dados.
- **label:** Fornece descrições para os campos.
- **select:** Cria uma lista suspensa.
- **textarea:** Permite a entrada de textos longos, como comentários ou mensagens.

**💡 Exemplo Analógico:**
Imagine um formulário HTML como um questionário em papel. Cada campo de entrada é uma pergunta, e o botão de envio é a entrega desse questionário para o servidor.

**Exemplo Prático:**

```html
<form action="processar.php" method="POST">
    <label for="nome">Nome:</label>
    <input type="text" id="nome" name="nome">
    
    <label for="mensagem">Mensagem:</label>
    <textarea id="mensagem" name="mensagem"></textarea>
    
    <label for="opcao">Escolha uma opção:</label>
    <select id="opcao" name="opcao">
        <option value="opcao1">Opção 1</option>
        <option value="opcao2">Opção 2</option>
    </select>
    
    <button type="submit">Enviar</button>
</form>
```

---

## **🌐 2. Métodos GET e POST - Como Utilizar**

Os métodos `GET` e `POST` são usados para enviar dados de formulários para o servidor, mas têm diferenças importantes.

### **🔄 Diferença entre GET e POST:**

- **GET:** Envia os dados diretamente na URL. Ideal para buscas ou ações simples.
- **POST:** Envia os dados no corpo da requisição. Ideal para envio de informações sensíveis.

**💡 Exemplo Analógico:**

- **GET:** Como escrever uma mensagem em um cartão postal (os dados ficam visíveis).
- **POST:** Como enviar uma carta em um envelope fechado (os dados ficam ocultos).

**Exemplo Prático (GET e POST):**

```php
// Usando GET
$nome = $_GET['nome'];
echo "Nome recebido via GET: " . $nome;

// Usando POST
$nome = $_POST['nome'];
echo "Nome recebido via POST: " . $nome;
```

---

## **💻 3. PHP (parte 9) - SESSION**

As `SESSIONs` no PHP permitem armazenar informações do usuário de forma temporária durante sua navegação no site.

### **🧠 Como Funcionam as Sessions:**

- **session\_start():** Inicia uma sessão.
- **$\_SESSION:** Superglobal usada para acessar e manipular os dados da sessão.
- **session\_unset():** Remove todas as variáveis de sessão.
- **session\_destroy():** Encerra a sessão.

**💡 Exemplo Analógico:**
Uma sessão é como um armário temporário em uma biblioteca. O usuário pode deixar seus pertences (dados) lá enquanto estiver usando os recursos do sistema.

**Exemplo Prático:**

```php
session_start();
$_SESSION['usuario'] = 'João';

// Acessando dados da sessão
echo "Usuário: " . $_SESSION['usuario'];

// Encerrando sessão
session_destroy();
```

---

## **📝 4. Proposta de Exercícios**

### **✅ Exercício 1:**

- **🎯 Objetivo:** Entender a estrutura de formulários HTML.
- **📝 Instrução:** Crie um formulário HTML com os seguintes campos:
  - Nome (input text)
  - Email (input email)
  - Mensagem (textarea)
  - Opção (select com pelo menos 3 opções).
    Ao enviar, os dados devem ser exibidos em uma página PHP usando o método `POST`.

### **✅ Exercício 2:**

- **🎯 Objetivo:** Utilizar métodos GET e POST.
- **📝 Instrução:** Crie duas páginas PHP:
  - A primeira deve capturar dados usando o método `GET` e exibir os valores.
  - A segunda deve capturar dados usando o método `POST` e exibir os valores.
    Use pelo menos três campos diferentes em cada método.

### **✅ Exercício 3:**

- **🎯 Objetivo:** Manipular sessões em PHP.
- **📝 Instrução:** Crie um sistema de login simples:
  - Página 1: Formulário com campo de login, senha e botão de login.
  - Página 2: Exiba uma mensagem de boas-vindas com o nome do usuário, armazenado na sessão.
  - Adicione um botão de logout que encerra a sessão.

# 🧠 Atividade: AJAX (Asynchronous JavaScript and XML)

Repositório desenvolvido em grupo para a atividade prática sobre **AJAX**, explorando diferentes formas de realizar requisições assíncronas no JavaScript.

---

## 👥 Integrantes do Grupo
| Nome | Função |
|------|--------|
| **Luiza Santiago** | Implementação com `async/await` e comparação entre métodos |
| **Cadu** | Pesquisa teórica sobre XmlHttpRequest, Fetch, Promises e Async/Await |
| **Nahiara** | Implementação usando Promises |
| **Ana** | Implementação usando Fetch API |
| **Ruan** | Comparação de desempenho e facilidade de uso |
| **Ismael** | Organização do repositório e formatação do README |

---

## 🧩 Estrutura do Repositório
```
ajax-comparativo-grupo/
│
├── ajax3_fetch.html        ← código da Ana
├── ajax3_promises.html     ← código da Nahiara
├── ajax3_async.html        ← código da Luiza
│
└── README.md               ← este arquivo
```

---

## 🧠 1️⃣ Introdução (por Cadu)
> 🔹 *Espaço reservado para Cadu preencher com a parte teórica.*  
> Deve explicar o que é AJAX, sua função, e como evoluiu (XmlHttpRequest → Fetch → Promises → Async/Await).

---

## ⚙️ 2️⃣ Código com Fetch API (por Ana)
> 🔹 *Espaço reservado para Ana descrever seu código `ajax3_fetch.html`.*  
> Incluir objetivo, passos principais e vantagens da Fetch API.

---

## 🔁 3️⃣ Código com Promises (por Nahiara)
> 🔹 *Espaço reservado para Nahiara explicar o código `ajax3_promises.html`.*  
> Descrever como as Promises foram usadas e os benefícios desse método.

---

## ⚡ 4️⃣ Código com Async/Await (por **Luiza**)

### 💡 Descrição do código `ajax3_async.html`
Este código implementa uma requisição AJAX utilizando **Async/Await**, uma forma moderna e simplificada de lidar com operações assíncronas em JavaScript.

O objetivo é buscar dados de um arquivo remoto (como `dados.json`) e exibi-los na página sem precisar recarregar todo o conteúdo.

### ⚙️ Funcionamento do código

1. A função é declarada com a palavra-chave `async`, indicando que ela conterá operações assíncronas.
2. Dentro dela, usamos `await` para **aguardar** a resposta da requisição feita com `fetch()`.
3. A resposta é convertida em JSON e exibida no console (ou inserida no HTML).
4. Todo o processo é envolvido em um bloco `try...catch` para tratar possíveis erros de rede.

### 🧩 Exemplo do código

```javascript
async function carregarDados() {
  try {
    const resposta = await fetch("dados.json");
    const dados = await resposta.json();
    document.getElementById("resultado").innerHTML = JSON.stringify(dados);
  } catch (erro) {
    console.error("Erro ao carregar os dados:", erro);
  }
}

carregarDados();
```

### ✅ Vantagens do uso de Async/Await
- **Código mais legível:** parece código síncrono, mesmo sendo assíncrono.  
- **Melhor tratamento de erros:** com `try...catch`, é fácil capturar falhas.  
- **Evita o “callback hell”** que acontecia com XmlHttpRequest e Promises aninhadas.  
- **Mais fácil de manter** e entender, especialmente em projetos grandes.

### ⚖️ Comparação com outros métodos

| Método             | Legibilidade | Complexidade | Tratamento de Erros | Indicado para |
|--------------------|--------------|---------------|---------------------|----------------|
| **XmlHttpRequest** | Baixa        | Alta          | Manual              | Sistemas antigos |
| **Fetch API**      | Alta         | Média         | Por `.catch()`      | Aplicações modernas |
| **Promises**       | Média        | Média         | `.then()` / `.catch()` | Uso intermediário |
| **Async/Await**    | **Muito alta** | **Baixa**    | `try...catch`       | Projetos atuais |

📘 **Conclusão da Luiza:**  
O uso de `async/await` simplifica o código, tornando o desenvolvimento mais rápido e legível.  
Além disso, combina bem com APIs modernas como `fetch`, sendo atualmente a **forma mais prática e recomendada** para trabalhar com AJAX no JavaScript.

---

## 📊 5️⃣ Comparação de Desempenho e Facilidade (por Ruan)
> 🔹 *Espaço reservado para Ruan.*  
> Incluir tabela ou gráfico comparando desempenho e facilidade entre `fetch`, `promises` e `async/await`.

---

## 🗂️ 6️⃣ Organização e Publicação (por Ismael)
> 🔹 *Espaço reservado para Ismael.*  
> Descrever como o repositório foi criado, configurado e publicado no GitHub (público, com README formatado e link enviado no Moodle).

---

## 🏁 Conclusão Geral (todo o grupo)
> 🔹 *Espaço para o grupo escrever a conclusão final.*  
> Sugestão: refletir sobre o aprendizado obtido, principais diferenças entre os métodos e qual abordagem consideram mais eficiente.

---

## ✍️ Observações Finais
> - Cada integrante deve revisar sua parte no README antes do envio.  
> - O arquivo deve estar formatado corretamente em Markdown.  
> - O repositório deve ser **público** e conter todos os arquivos `.html` e este README.

---

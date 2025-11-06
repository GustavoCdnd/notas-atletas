# 🏅 Média dos Atletas

Um projeto simples em **JavaScript** que calcula a **média válida** das notas de cada atleta, **eliminando a maior e a menor nota** antes do cálculo.  
Ideal para praticar **laços de repetição**, **arrays**, **métodos como `.sort()`, `.slice()` e `.forEach()`**, e manipulação de dados em JS.

---

📜 Descrição

O programa percorre uma lista de atletas, ordena suas notas em ordem crescente, elimina a menor e a maior nota, e depois calcula a média das três notas restantes.  
Por fim, exibe no console o nome do atleta, suas notas ordenadas e a média final calculada.

---

## 💻 Tecnologias utilizadas
- 🟨 **JavaScript**


---

## 🚀 Como executar

1. Crie um arquivo chamado `atletas.js`
2. Copie o código abaixo:

   ```js
   let atletas = [
     { nome: "Cesar Abascal", notas: [10, 9.34, 8.42, 10, 7.88] },
     { nome: "Fernando Puntel", notas: [8, 10, 10, 7, 9.33] },
     { nome: "Daiane Jelinsky", notas: [7, 10, 9.5, 9.5, 8] },
     { nome: "Bruno Castro", notas: [10, 10, 10, 9, 9.5] }
   ];

   for (let atleta of atletas) {
     let notas = atleta.notas.sort((a, b) => a - b);
     let notasComputadas = notas.slice(1, 4);
     let soma = 0;

     for (let nota of notasComputadas) {
       soma += nota;
     }

     let media = soma / notasComputadas.length;

     console.log(`Atleta: ${atleta.nome}`);
     console.log(`Notas Obtidas: ${notas.join(",")}`);
     console.log(`Média Válida: ${media}`);
     console.log("");
   }
   ```

3. Execute o arquivo com o Node.js:
   ```bash
   node atletas.js
   ```

4. Veja a saída no console 🎯

---

## 🧮 Exemplo de saída

```
Atleta: Cesar Abascal
Notas Obtidas: 7.88,8.42,9.34,10,10
Média Válida: 9.253333333333334

Atleta: Fernando Puntel
Notas Obtidas: 7,8,9.33,10,10
Média Válida: 9.11

Atleta: Daiane Jelinsky
Notas Obtidas: 7,8,9.5,9.5,10
Média Válida: 9

Atleta: Bruno Castro
Notas Obtidas: 9,9.5,10,10,10
Média Válida: 9.833333333333334
```

---

## 📂 Estrutura do projeto

```
📁 media-dos-atletas
│
├── atletas.js      # Código principal
└── README.md       # Documentação do projeto
```

---

## 🧠 Conceitos praticados
- Uso de **loops (`for`, `for...of`)**
- Manipulação de **arrays**
- Métodos: `.sort()`, `.slice()`, `.forEach()`, `.join()`
- Cálculo de **médias**
- Saída formatada com **template strings**

---

## 👨‍💻 Autor
**Gustavo**  
📍 Desenvolvedor em aprendizado  
📧 Contato: lucasgustavodss@gmail.com*

---

✨ _"Estudando bastante para entender tudo, pois é dificultoso lembrar de tudo mas a pratica sempre vai levar a melhora."_  

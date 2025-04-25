# Temperatura, Top-k e Top-p

## 🔥 Temperatura (`temperature`)

**O que é:** Controla o nível de aleatoriedade na escolha das palavras.

| Temperatura | Comportamento            | Exemplo prático                    |
| ----------- | ------------------------ | ---------------------------------- |
| 0.0         | Ultra determinístico     | Sempre responde igual              |
| 0.7         | Equilíbrio criativo      | Criatividade com coerência         |
| 1.0+        | Bem criativo (e caótico) | Pode sair engraçado ou sem sentido |

✅ Use temperatura baixa quando quiser respostas exatas ou técnicas (ex: atendimento farmacêutico).  
✅ Use temperatura média/alta em casos de brainstorming, escrita criativa ou storytelling.

---

## 🧮 Top-k (`top_k`)

**O que é:** Define quantas opções o modelo considera antes de escolher a próxima palavra.

| Top-k | Comportamento                       |
| ----- | ----------------------------------- |
| 0     | Considera todas as opções           |
| 20    | Considera só as 20 mais prováveis   |
| 100   | Ainda criativo, mas menos aleatório |

✅ Útil para limitar variações exageradas, especialmente em textos informativos.

---

## 🎲 Top-p (`top_p`, ou _nucleus sampling_)

**O que é:** Em vez de número fixo (top-k), ele soma as probabilidades até passar um certo limiar.

| Top-p | Comportamento                                |
| ----- | -------------------------------------------- |
| 1.0   | Não filtra nada                              |
| 0.9   | Considera só as palavras com 90% cumulativas |
| 0.5   | Considera apenas palavras muito prováveis    |

✅ Mais flexível e natural do que top-k.  
✅ Funciona melhor quando a temperatura está moderada (0.6 a 0.8).

---

## 🧠 Combinações ideais

| Cenário                           | Temperatura | Top-k | Top-p | Resultado                             |
| --------------------------------- | ----------- | ----- | ----- | ------------------------------------- |
| Atendimento técnico (RAG)         | 0.0         | 0     | 1.0   | Totalmente confiável e estável        |
| Chat natural, amigável            | 0.7         | 40    | 0.9   | Equilíbrio entre coerência e variação |
| Escrita criativa (história)       | 1.0         | 100   | 0.95  | Mais ousado e imaginativo             |
| Explicação didática com variações | 0.5         | 50    | 0.8   | Mais diverso, sem fugir do foco       |

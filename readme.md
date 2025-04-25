# 📘 Engenharia de Prompt com Técnicas Avançadas

---

## Índice

1. [Tom, Persona e Estilo de Escrita](#1-tom-persona-e-estilo-de-escrita)
2. [5 Passos para Simulações Eficazes](#2-5-passos-para-simulações-eficazes)
3. [O que é um Playbook](#3-o-que-é-um-playbook)
4. [Prompt Criativo vs Prompt Factual](#4-prompt-criativo-vs-prompt-factual)
5. [Chain-of-Thought](#5-chain-of-thought)
6. [Zero-shot, One-shot e Few-shot](#6-zero-shot-one-shot-e-few-shot)
7. [Instruções Diretas vs Indiretas](#7-instruções-diretas-vs-indiretas)
8. [Temperatura, Top-k e Top-p](#8-temperatura-top-k-e-top-p)
9. [Janela de Contexto e Resumo](#9-janela-de-contexto-e-resumo)
10. [Mitigação de Alucinações com Prompting](#10-mitigação-de-alucinações-com-prompting)
11. [Performance e Clareza](#11-performance-e-clareza)

---

## 1. Tom, Persona e Estilo de Escrita

| Elemento    | Descrição                        | Exemplo                         |
| ----------- | -------------------------------- | ------------------------------- |
| **Tom**     | Emoção e formalidade da resposta | Informal, Técnico, Acolhedor    |
| **Persona** | Quem "fala" com o usuário        | Médico, Farmacêutico, Professor |
| **Estilo**  | Estrutura, vocabulário e fluidez | Simples, Elaborado, Criativo    |

Ajustar esses elementos ajuda o modelo a responder com mais aderência ao público.

---

## 2. 5 Passos para Simulações Eficazes

### 1. Defina o cenário (contexto)

O que está acontecendo? Onde? Quando?

A situação deve ser clara e contextualizada.

Exemplo: "Você é um farmacêutico atendendo a um paciente em uma farmácia."

### 2. Escolha a persona (quem está falando ou agindo)

O papel ou identidade da IA.

Exemplo de personas: Farmacêutico, professor, atendente de suporte, líder de equipe, etc.

Exemplo: "Você é um farmacêutico com 5 anos de experiência e paciência para explicar com calma."

### 3. Determine o objetivo da simulação

O que a IA precisa fazer na simulação?

Objetivos comuns: Responder perguntas, solucionar problemas, dar conselhos, ensinar algo, etc.

Exemplo: "Explique ao paciente como tomar um remédio corretamente."

### 4. Estabeleça parâmetros (restrições ou desafios)

Pode ser um problema ou restrição no cenário que a IA deve superar.

Exemplo: "O paciente tem dificuldade de leitura e não consegue entender instruções complexas."

### 5. Adapte a linguagem e o tom

Ajuste para que a IA fale de maneira apropriada para o público-alvo.

Exemplo de tom: Amigável, formal, urgente, calmo, etc.

---

## 3. O que é um Playbook

Um **playbook** é um guia estruturado com exemplos, padrões e estratégias para uso de prompts.  
Ele organiza o conhecimento e **acelera a criação de aplicações com IA**, mantendo a **consistência** e **eficiência**.

---

## 4. Prompt Criativo vs Prompt Factual

| Tipo     | Objetivo                         | Características                     |
| -------- | -------------------------------- | ----------------------------------- |
| Criativo | Gerar ideias, narrativas         | Alta temperatura, tom fluido        |
| Factual  | Buscar precisão e dados corretos | Temperatura baixa, linguagem direta |

---

## 5. Chain-of-Thought

Técnica para forçar o modelo a **"pensar em voz alta"**, quebrando o raciocínio em etapas.  
**Exemplo:**

> "Para resolver isso, primeiro analisamos X, depois comparamos com Y, e então concluímos Z."

---

## 6. Zero-shot, One-shot e Few-shot

| Técnica   | Descrição             | Exemplo                                  |
| --------- | --------------------- | ---------------------------------------- |
| Zero-shot | Nenhum exemplo dado   | "Resuma esse texto."                     |
| One-shot  | Um exemplo dado       | "Como nesse exemplo, faça o mesmo."      |
| Few-shot  | Vários exemplos dados | "Veja estes exemplos e repita o padrão." |

---

## 7. Instruções Diretas vs Indiretas

| Tipo     | Exemplo                                                  |
| -------- | -------------------------------------------------------- |
| Direta   | "Liste os benefícios do paracetamol."                    |
| Indireta | "Se eu estiver com dor de cabeça, o que pode me ajudar?" |

---

## 8. Temperatura, Top-k e Top-p

| Parâmetro   | Função                               | Efeito                           |
| ----------- | ------------------------------------ | -------------------------------- |
| Temperatura | Aleatoriedade da resposta            | Alta = criativo, Baixa = preciso |
| Top-k       | Considera os k tokens mais prováveis | k baixo = conservador            |
| Top-p       | Tokens até atingir p% acumulado      | p baixo = previsível             |

**Combinações ideais:**

- Criatividade: `Temperatura 0.8`, `Top-p 0.95`
- Precisão: `Temperatura 0.2`, `Top-p 0.7`

---

## 9. Janela de Contexto e Resumo

| Elemento           | Impacto                                   |
| ------------------ | ----------------------------------------- |
| Janela de contexto | Limita quantos tokens o modelo pode "ver" |
| Resumo             | Compressão do contexto mantendo o sentido |

---

## 10. Mitigação de Alucinações com Prompting

- Use **instruções claras e específicas**
- Solicite **fontes ou justificativas**
- Combine com **RAG** para trazer fatos externos
- Reduza **temperatura** e aumente **controle** no prompt

---

## 11. Performance e Clareza

- **Menos tokens** = respostas mais rápidas e diretas
- **Frases longas ou mal escritas** afetam o desempenho
- Clareza e estrutura no prompt garantem **melhor performance**

💡 _Dica: revise os prompts como se estivesse explicando para uma criança ou escrevendo um tweet._

---

# Zero-shot, One-shot e Few-shot

### O que são?

Essas técnicas descrevem diferentes abordagens de **como fornecer exemplos** ao modelo para que ele realize uma tarefa específica.

### Explicação:

| Técnica       | Descrição                                                                                      | Exemplo                                                                         |
| ------------- | ---------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **Zero-shot** | Nenhum exemplo fornecido. O modelo precisa realizar a tarefa sem qualquer referência anterior. | "Resuma este texto."                                                            |
| **One-shot**  | Um único exemplo é dado para o modelo. O modelo tenta seguir o padrão com base nesse exemplo.  | "Como neste exemplo, faça o mesmo: [exemplo]."                                  |
| **Few-shot**  | Vários exemplos são fornecidos para o modelo aprender o padrão e realizar a tarefa.            | "Veja esses exemplos e repita o padrão: [exemplo 1], [exemplo 2], [exemplo 3]." |

### Quando usar?

- **Zero-shot**: Quando você quer que o modelo execute uma tarefa sem precisar de exemplos prévios. Útil quando o modelo tem um bom entendimento geral da tarefa.
- **One-shot**: Quando você tem um único exemplo claro e deseja que o modelo faça algo similar.
- **Few-shot**: Quando a tarefa é complexa ou precisa de maior contexto. Ao fornecer múltiplos exemplos, você ajuda o modelo a entender melhor o padrão.

### Benefícios:

- **Zero-shot**: Maior flexibilidade e agilidade para tarefas inéditas.
- **One-shot**: Útil para quando um exemplo é suficiente para entender o padrão.
- **Few-shot**: Melhora a precisão e adequação para tarefas mais específicas ou difíceis.

---

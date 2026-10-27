# 🗣️ Avaliação de Comunicabilidade

## Método Utilizado:

<div align="justify">

O **Método de Avaliação de Comunicabilidade (MAC)** é uma técnica de inspeção de usabilidade baseada na Engenharia Semiótica. Em vez de focar apenas na facilidade de uso, o MAC avalia a qualidade da comunicação entre o designer do sistema e o usuário final, intermediada pela interface. O objetivo é descobrir se o usuário consegue entender a lógica, as intenções e as soluções que o designer embutiu no software.

A avaliação geralmente envolve a gravação de usuários realizando tarefas específicas, seguida da anotação das interações.

---

### Rupturas de Comunicabilidade (Etiquetas)

As rupturas de comunicabilidade ocorrem quando a mensagem do designer falha em chegar ao usuário. No MAC, essas quebras de comunicação são categorizadas usando "etiquetas" (tags) que representam a reação ou o pensamento do usuário no momento da falha.

Abaixo estão as principais rupturas mapeadas pelo método:

| Etiqueta (Ruptura) | O que o usuário expressa / sente | O que acontece na prática |
| --- | --- | --- |
| **Desisto** | "Não consigo concluir esta tarefa." | O usuário explicitamente admite não conseguir concluir uma tarefa. |
| **Para mim está bom...** | "Terminei a tarefa com sucesso." | O usuário equivocadamente acredita que concluiu a tarefa. |
| **Não, obrigado.** | "Prefiro seguir por outro caminho." | O usuário decide seguir por um caminho não preferido pelo designer, mesmo conhecendo o caminho preferido e sabendo como percorrê-lo. |
| **Vai de outro jeito.** | "Não consigo seguir o caminho recomendado, vou tentar outro." | O usuário não conhece, ou não consegue percorrer, o caminho de interação preferido pelo designer e então é obrigado a seguir outro caminho de interação. |
| **Cadê?** | "Onde está a função que eu preciso?" | O usuário não consegue expressar sua intenção através dos signos codificados na interface. |
| **Ué, o que houve?** | "O que aconteceu? Não entendi a resposta do sistema." | O usuário não percebe ou não compreende as respostas do sistema decorrentes de uma ação anterior. |
| **E agora?** | "Qual é o próximo passo?" | O usuário não sabe o que fazer em determinado momento para concluir uma tarefa. |
| **Onde estou?** | "Por que não consigo fazer isso nesta etapa?" | O usuário tenta dizer algo que o sistema é capaz de entender em outro contexto, diferente do atual. |
| **Epa!** | "Cometi um erro, preciso desfazê-lo." | O usuário cometeu um equívoco, percebe o engano e tenta desfazê-lo. |
| **Assim não dá.** | "Esse caminho é improdutivo, vou parar." | O usuário interrompe e abandona um caminho de interação com vários passos por considerá-lo improdutivo. |
| **O que é isto?** | "Para que serve este botão ou ícone?" | O usuário não consegue interpretar o significado dos signos estáticos e dinâmicos codificados na interface. |
| **Socorro!** | "Preciso de ajuda para concluir esta tarefa." | O usuário consulta a ajuda online ou outras fontes de informação e explicação para concluir as tarefas. |
| **Por que não funciona?** | "Por que o sistema não apresentou o resultado esperado?" | O usuário esperava obter determinados resultados do sistema e não entende por que o sistema produziu resultados diferentes do esperado. |

Essas etiquetas são fundamentais para diagnosticar exatamente onde o design falha em guiar as ações e expectativas de quem está usando a plataforma.

---

## Participantes e Tarefas:

### Rosaura Oliveira.
### Maria Caroline

---

## Registro das Seções:

### [Apresentar o link dos vídeos]

- [Vídeo do participante Maria Caroline](https://classroom.google.com/h/st)
- [Vídeo do participante Rosaura Oliveira](https://classroom.google.com/h/st)

---

## Etiquetagem das Rupturas

A avaliação de usabilidade baseada no método MAC identificou falhas graves de comunicação na interface que geram frustração e impedem a conclusão de tarefas. Os principais problemas diagnosticados foram:

Cadastro longo e confuso: Usuários pulam etapas frequentemente devido à má progressão ou exigência de dados desnecessários.

Falta de feedback visual: O sistema não confirma o sucesso de ações como login, configurações ou término de tarefas, deixando o usuário em dúvida.

Bloqueios de navegação ("Becos sem saída"): Telas críticas, como a de validação do PIX, não possuem botões de cancelamento ou retorno, forçando a desistência.

Problemas de descoberta: Recursos básicos, como barra de busca e favoritar eventos, estão ocultos ou difíceis de encontrar.

Erros não explicados: Falta de clareza nos requisitos para a publicação de eventos leva ao abandono da tarefa.

Conclusão: Para corrigir esses atritos, a interface precisa simplificar a jornada de cadastro, fornecer respostas visuais imediatas após cada interação e garantir rotas de fuga claras (botões de voltar/cancelar), especialmente em modais e telas de pagamento.

| Participante | Tarefa | Tela/Elementos | Situação Observada | Tipo de Falha | Etiqueta | Problema de Comunicabilidade |
|:----:|:----:|:----:|:----:|:----:|:----:|:----:| 
|Rosaura Oliveira|T1|Tela inicial|“foi ? foi !”|Temporário|Ué, o que houve?|Usuário não percebe que já está na conta|
|Rosaura Oliveira|T2|Tela de cadastro|“continuar cadastro”|Temporário|Não, obrigado. |Usuário pulou uma etapa do cadastro|
|Rosaura Oliveira|T2|Tela de cadastro|“foi?”|Temporário|Não, obrigado. |Novamente pulou uma etapa do cadastro|
|Rosaura Oliveira|T3|Tela inicial|“opa”|Temporário|Epa!|Usuário clicou em uma opção errada e voltou|
|Rosaura Oliveira|T4|Tela de um evento|“aham eu copiei o link...”|Temporário|Vai de outro jeito.|Usuário guardou o evento copiando seu link e não usando a opção favoritar pois não foi achada |
|Rosaura Oliveira|T5|Tela de um evento|“Não era isso?”|Temporário|Para mim está bom...|Usuário acredita ter terminado a tarefa|
|Rosaura Oliveira|T5|Tela de um evento|“Não foi só...”|Temporário|Ué, o que houve? |Usuário não entende que a tarefa não foi realizada após conclusão dos dados da sua conta|
|Rosaura Oliveira|T6|Tela de validar pix|“Tá eu não consegui”|Temporário|Desisto|Usuário não conseguiu sair da tela usando os recursos do sistema|
|Rosaura Oliveira|T9|Tela de criar evento|“Não tá dando pra publicar..”|Temporário|Por que não funciona?|Usuário esperava a criação de um evento porém não compreende inicialmente o motivo|
|Rosaura Oliveira|T9|Tela de criar eventos|“Desisto”|Temporário|Desisto|Usuário não consegue concluir a tarefa|
|Rosaura Oliveira|T10|Tela de ajuda para produtos|Não aplicável|Temporário|Onde estou? |Usuário segue um caminho alternativo ao central de ajuda|

| Participante | Tarefa | Tela/Elementos | Situação Observada | Tipo de Falha | Etiqueta | Problema de Comunicabilidade |
|:----:|:----:|:----:|:----:|:----:|:----:|:----:| 
|Maria Caroline|T2|Tela de cadastro|Não aplicável|Temporário|Não, obrigado.|Usuário pula uma etapa do cadastro|
|Maria Caroline|T2|Tela de cadastro|Não aplicável|Temporário|Não, obrigado.|Usuário pulou outra etapa do cadastro|
|Maria Caroline|T3|Tela inicial|“Ou sou eu que não sei usar?”|Temporário|E agora?|Usuário não entende como prosseguir para terminar a tarefa|
|Maria Caroline|T3|Tela inicial|Não aplicável|Temporário|Cadê?|Usuário não consegue identificar um método de busca|
|Maria Caroline|T4|Tela de um evento|“Puxa mas não aparece”|Temporário|Ué, o que houve?|Após algumas configurações o usuário esperava uma resposta/alteração que não apareceu|
|Maria Caroline|T4|Tela de um evento|Não aplicável|Temporário|Assim não dá.|Usuário mudou tipo de conta para poder realizar uma ação|
|Maria Caroline|T4|Tela de um evento|“Pois é não vai”|Temporário|Por que não funciona?|Mesmo fazendo as devidas alterações, o sistema não responde de forma apropriada resultado, tarefa não terminada por isso|
|Maria Caroline|T6|Tela de validação de pix|“Não, vou desistir”|Temporário|Desisto|Usuário não conseguiu sair da tela com os recursos do sistema|

## Consolidação das Etiquetas

A avaliação MAC revelou falhas críticas de usabilidade no sistema, concentrando os atritos mais severos nas Tarefas 2, 4, 6 e 9. Os principais problemas diagnosticados incluem:

Rejeição de etapas (T2): Ocorrência frequente de pulos no fluxo de cadastro, indicando excesso de passos ou solicitação de dados percebidos como desnecessários.

Ausência de feedback (T1, T4, T5): Falta de respostas visuais do sistema após interações, deixando o usuário confuso sobre o status de suas ações.

Bloqueios severos (T6, T9): Presença de "becos sem saída" na interface que impedem o progresso e forçam o usuário a abandonar a tarefa (desistência).

Navegação e Inconsistência (T3, T4, T9, T10): Dificuldade em localizar recursos básicos (como buscas) e respostas inesperadas do sistema frente às ações executadas.

As correções de design devem priorizar a simplificação do fluxo de cadastro (T2), a inclusão de feedback visual claro (T1, T4, T5) e o fornecimento de rotas de fuga para evitar o abandono em telas críticas (T6, T9).


| Etiqueta | Ocorrências (Rosaura Oliveira) | Ocorrências (Maria Caroline) | Total | Tarefas mais afetadas |
|:----:|:----:|:----:|:----:|:----:|
| Não, obrigado. | 2 | 2 | 4 | T2 |
| Ué, o que houve? | 2 | 1 | 3 | T1, T4, T5 |
| Desisto | 2 | 1 | 3 | T6, T9 |
| Por que não funciona? | 1 | 1 | 2 | T4, T9 |
| Epa! | 1 | 0 | 1 | T3 |
| Vai de outro jeito. | 1 | 0 | 1 | T4 |
| Para mim está bom... | 1 | 0 | 1 | T5 |
| Onde estou? | 1 | 0 | 1 | T10 |
| E agora? | 0 | 1 | 1 | T3 |
| Cadê? | 0 | 1 | 1 | T3 |
| Assim não dá. | 0 | 1 | 1 | T4 |

Etiquetas mais frequentes: As rupturas de comunicação mais comuns foram "Não, obrigado." (associada à rejeição de etapas de cadastro), "Ué, o que houve?" (refletindo a ausência de feedback visual) e "Desisto" (indicando falhas críticas e bloqueios severos de navegação).

Tarefas com mais rupturas: Os atritos mais severos concentraram-se nas tarefas T2 (fluxo de cadastro excessivo), T4 e T5 (ações sem confirmação de estado), além da T6 e T9 (telas com becos sem saída e erros não explicados).

Comunicação entre o sistema e os usuários: Os resultados indicam que a comunicação do sistema é falha e não suporta adequadamente o usuário durante sua jornada. O sistema gera confusão ao omitir respostas visuais após interações, exige dados percebidos como desnecessários e falha em fornecer rotas de fuga ou explicações claras em momentos críticos, o que rompe o diálogo interativo e força o abandono das tarefas.

<div>

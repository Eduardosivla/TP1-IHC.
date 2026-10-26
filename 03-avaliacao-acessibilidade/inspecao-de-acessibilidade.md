# ♿ Avaliação de Acessibilidade

<div align="justify">
A ideia principal de Acessibilidade em uma interface é garantir que a mesma não crie barreiras de uso. O objetivo da etapa não se trata apenas de testar um recurso em específico voltado as pessoas com deficiências físicas, mas sim auditar as funcionalidades normais do sistema (como buscar um evento, selecionar um ingresso ou fazer login) e verificar se elas podem ser operadas por qualquer pessoas, independentemente da limitação visual, cognitiva ou motoras.

<br>


## 🎯 Escopo da avaliação
Para estruturar essas inspeção no Sympla, usou-se como base os critérios da WCAG 2.2 (Diretrizes de Acessibilidade para Conteúdo Web). O processo combinou algumas ferramentas automatizadas - como leitores de tela do dispositivo - com testes manuais baseados na prática do usuário. Para os testes, foram selecionadas as seguintes telas: 

| Tela | Descrição |
| :--- | :--- |
| **Página Inicial e Busca** | Tela de entrada do sistema, incluindo a barra de pesquisa de eventos e os filtros de calendário explorados durante os testes. |
| **Detalhes do Evento** | Página de apresentação de um evento específico, englobando as informações gerais, os botões de seleção de ingresso e o rodapé da plataforma. |
| **Minha Conta** | Área restrita de gerenciamento do perfil do usuário logado e acompanhamento de ingressos. |
| **Pagamento (Checkout)** | Fluxo de finalização do pedido, contemplando os formulários de preenchimento, caixas de seleção e métodos de transação como o PIX. |

<br>

## ⚙️ Processo utilizado

Para estruturar o processo de inspeção e garantir uma maior cobertura de falhas, dividiu-se o trabalho em três etapas metodológicas: detecção, coleção e discriminação.

---

**1. Detecção**

Numa primeira fase, realizaram-se inspeções individuais e independentes nas páginas selecionadas do sistema. Cada avaliador testou a interface por conta própria, utilizando o roteiro estabelecido - como a navegação exclusiva por teclado, leitores de ecrã e ferramentas de contraste automatizadas. O objetivo não se tratava de criar um consenso imediato, mas sim de registar individualmente o máximo de barreiras que violassem as diretrizes da WCAG.

---

**2. Coleção**

Após a conclusão das análises individuais, reuniram-se todos os apontamentos num único documento de controlo. Como era esperado numa avaliação colaborativa, identificaram-se diversos registos sobrepostos, onde vários membros da equipa relataram de forma isolada o mesmo problema - como a perda de componentes ao utilizar o zoom ou a ausência de contraste adequado no rodapé.

---

**3. Discriminação**
Por fim, organizou-se uma sessão conjunta para debater os dados recolhidos. O objetivo desta etapa final tratou-se de unificar os registos duplicados e debater os falsos positivos (situações que aparentavam ser erros visuais, mas que não violavam estritamente os critérios da WCAG 2.2). O consenso gerado após este filtro formou a lista oficial de defeitos consolidados que se apresenta a seguir.

<br>

## 📊 Resultados da inspeção

Entre as principais fragilidades identificadas, destaca-se os problemas de operação por teclado e o comportamento do sistemas diante de tecnologias assistivas. A interrupção do foco da navegação em componentes essenciais, como a barra de busca e botões de seleção de ingressos que inviabiliza a conclusão de tarefas fundamentais para usuários com limitações motoras. Além disso, existe no sistema a ausência da padronização nas etiquetas interpretadas pelos leitores de tela - Orca, o utilizado para o teste - que comprometem a navegação de pessoas com deficiências visuais.

No aspecto visual do site, observaram-se falhas recorrentes relacionados a perceptibilidade. O baixo contraste entre textos e fundo (presente em detalhes do evento, elementos do rodapé e áreas de fluxo de pagamento) que dificulta a leitura para pessoas com baixa visão. Da mesma maneira, o comportamento da interface ao aplicar o redimensionamento de tela (zoom 200%) revelou problemas de retorno e sobreposição de componentes, resultando na perda de visibilidade de campos importantes ao avançar para etapas posteriores.

---
<br>

### 🚨 Síntese dos problemas encontrados

<div align="justify">
  
A tabela a seguir apresenta a síntese das falhas identificadas durante a avaliação, detalhando a descrição do problema, o critério da WCAG violado, a página onde a ocorrência foi detetada e a respetiva frequência observada durante os testes.

</div>

| Problema | Critério WCAG | Tela/Página | Frequência |
| :--- | :--- | :--- | :---: |
| Interrupção da navegação por teclado na barra de pesquisa e botões de ação | 2.1.1 - Teclado | Página Inicial / Detalhes | 3 |
| Contorno de foco invisível ou com contraste insuficiente em elementos interativos | 2.4.7 - Foco Visível | Várias | 2 |
| Rótulos genéricos e sem contexto interpretados pelo leitor de ecrã | 4.1.2 - Nome, Função, Valor | Várias | 3 |
| Perda de conteúdo, corte de elementos e sobreposição ao aplicar zoom de 200% | 1.4.10 - Refluxo | Várias | 4 |
| Anulação automática do zoom aplicado pelo utilizador na transição para o pagamento | 1.4.4 - Redimensionamento de texto | Pagamento | 1 |
| Fontes finas e claras sobre fundos claros que dificultam a leitura | 1.4.3 - Contraste mínimo | Detalhes / Pagamento / PIX | 4 |
| Falta de contraste delimitador em caixas de texto, barras e ícones | 1.4.11 - Contraste não textual | Várias | 3 |
| Dependência exclusiva de cor para identificação de hiperligações e estados | 1.4.1 - Uso da cor | Rodapé / Formulários | 2 |

---

<br>

### 📜 Critérios WCAG violados

<div align="justify">
  
A tabela seguinte sintetiza a distribuição dos critérios oficiais da WCAG 2.2 que foram violados, categorizados pelos seus respetivos princípios e diretrizes de acessibilidade, bem como o nível de conformidade associado.

</div>

| Princípio | Diretriz | Critério violado | Nível |
| :--- | :--- | :--- | :---: |
| Perceptível | 1.4 Distinguível | 1.4.1 Uso da Cor | A |
| Perceptível | 1.4 Distinguível | 1.4.3 Contraste mínimo | AA |
| Perceptível | 1.4 Distinguível | 1.4.4 Redimensionamento de texto | AA |
| Perceptível | 1.4 Distinguível | 1.4.10 Refluxo | AA |
| Perceptível | 1.4 Distinguível | 1.4.11 Contraste não textual | AA |
| Operável | 2.1 Acessível por teclado | 2.1.1 Teclado | A |
| Operável | 2.4 Navegável | 2.4.7 Foco visível | AA |
| Robusto | 4.1 Compatível | 4.1.2 Nome, Função, Valor | A |

<br>

## 💡 Considerações sobre os resultados

<div align="justify">
  
A partir dos dados recolhidos, observou-se que o sistema apresenta fragilidades significativas na adequação para utilizadores que dependem de tecnologias assistivas ou navegação exclusiva por teclado. As "barreiras" de contraste visual e o comportamento inadequado da interface perante o redimensionamento (zoom) demonstram que, embora a plataforma seja funcional no cenário padrão, carece de robustez técnica para garantir uma experiência inclusiva. Destaca-se, contudo, o cumprimento pontual de critérios como a exibição de mensagens de erro textuais em formulários e o escurecimento de imagens de fundo sob texto.

</div>

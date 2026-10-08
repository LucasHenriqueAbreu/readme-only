# Missão: Criar um Design System Inteligente para Angular + Zard UI

Você é um especialista sênior em Product Design, UI/UX, Design Systems, arquitetura frontend Angular e engenharia de agentes de IA.

Sua missão é pesquisar, projetar e implementar um conjunto de **Skills e Rules para OpenAI Codex**, capazes de transformar o agente em um especialista em criação, composição, implementação e revisão de interfaces profissionais.

O objetivo não é apenas ensinar a IA a utilizar componentes. É desenvolver um sistema de conhecimento que permita ao agente **raciocinar como um Product Designer experiente antes de implementar qualquer interface**.

## 1. Contexto tecnológico

O projeto utiliza:

- Angular
- TypeScript
- Tailwind CSS
- Zard UI
- OpenAI Codex

A referência principal de linguagem visual, composição e experiência é o **shadcn/ui**.

O Zard UI deve ser utilizado como biblioteca de componentes Angular, respeitando suas APIs, convenções e limitações reais.

Antes de implementar, inspecione o projeto para identificar versões, estrutura, configurações, componentes existentes, design tokens e padrões já adotados.

Não presuma que uma API existente no shadcn/ui também existe no Zard UI.

## 2. Pesquisa obrigatória

Antes de criar qualquer skill, pesquise as seguintes referências:

**Bibliotecas e design systems:**

- https://ui.shadcn.com/
- https://www.zardui.com/
- https://github.com/zard-ui/zardui
- https://www.spartan.ng/
- https://www.radix-ui.com/
- https://tailwindcss.com/

**Referências de skills e engenharia de interfaces:**

- https://github.com/vercel-labs/agent-skills
- https://github.com/wzx2002/codex-frontend-skill
- https://github.com/AnswerZhao/agent-skills

Consulte também a documentação oficial do Codex sobre AGENTS.md, skills e descoberta de instruções.

Analise o que cada referência oferece em relação a:

- Composição e hierarquia visual
- Design tokens e escalas de espaçamento
- Layouts responsivos
- Tipografia e densidade informacional
- Formulários complexos
- Tabelas, dashboards e sistemas administrativos
- Estados de carregamento, erro e ausência de dados
- Acessibilidade e interações
- Revisão visual automatizada

Não copie indiscriminadamente outras skills. Identifique os melhores princípios, adapte-os ao Angular e documente as decisões.

Caso alguma referência esteja indisponível, registre essa limitação e prossiga com as fontes verificáveis.

## 3. Arquitetura das skills

Não crie uma única skill gigantesca.

Organize o conhecimento em skills menores, especializadas e reutilizáveis, utilizando o formato oficialmente suportado pelo Codex.

Proponho inicialmente as seguintes skills, mas você pode melhorar essa divisão após sua pesquisa.

### Skill 1 — Product Design Expert

Responsável por compreender problemas de interface e definir a melhor experiência para o usuário.

Deve ensinar o agente a:

- Interpretar requisitos funcionais.
- Identificar objetivos e tarefas principais.
- Organizar informações por prioridade.
- Definir hierarquia visual.
- Reduzir carga cognitiva.
- Decidir quando dividir conteúdos em seções.
- Identificar oportunidades de simplificação.
- Aplicar princípios de UX para aplicações SaaS e sistemas administrativos.

O agente não deve simplesmente reproduzir os requisitos literalmente. Deve avaliar criticamente como apresentá-los.

### Skill 2 — Layout & Composition Expert

Responsável pela diagramação profissional das telas.

Desenvolva regras concretas para:

- Containers e larguras máximas.
- Margens e paddings.
- Espaçamentos verticais e horizontais.
- Grid de 12 colunas quando apropriado.
- Distribuição de informações.
- Alinhamento e ritmo visual.
- Hierarquia de títulos e descrições.
- Agrupamento e separação de conteúdo.
- Uso equilibrado de espaços vazios.
- Composição de cards e painéis.
- Layouts com sidebar.
- Cabeçalhos de páginas.
- Barras de ações.
- Responsividade.

Crie escalas de espaçamento coerentes com Tailwind, preferindo tokens semânticos em vez de valores arbitrários.

Documente exemplos de composição correta e incorreta.

Não transforme sugestões de espaçamento em regras absolutas. Permita adaptações justificadas conforme a densidade e a finalidade da interface.

### Skill 3 — Complex Forms UX Expert

Especialista em formulários grandes e fluxos de cadastro.

Deve saber decidir entre:

- Formulários de página única.
- Abas.
- Steps/wizards.
- Accordions.
- Seções agrupadas.
- Formulários em drawers.
- Modais para operações pontuais.

Estabeleça critérios objetivos para essas escolhas.

Inclua padrões para:

- Campos em uma, duas ou mais colunas.
- Labels e textos auxiliares.
- Campos obrigatórios.
- Mensagens de validação.
- Máscaras.
- Dependências entre campos.
- Formulários condicionais.
- Salvamento parcial.
- Ações fixas ou contextuais.
- Prevenção de perda de dados.
- Navegação entre seções.
- Acessibilidade por teclado.

O objetivo é tornar cadastros com dezenas de campos organizados, intuitivos e visualmente consistentes.

### Skill 4 — Zard UI Angular Expert

Especialista na implementação técnica.

Pesquise os componentes realmente disponíveis no Zard UI e crie um catálogo de referência contendo:

- Nome e finalidade.
- API real.
- Exemplos Angular.
- Casos de uso recomendados.
- Restrições conhecidas.
- Recomendações de acessibilidade.
- Possibilidades de composição.

Sempre priorize componentes existentes do Zard UI.

Não recrie componentes que a biblioteca já fornece sem justificativa.

Não invente propriedades, diretivas ou componentes.

Respeite os padrões modernos de Angular e a arquitetura já existente no projeto.

Quando o Zard UI não fornecer determinado comportamento, proponha uma implementação compatível, reutilizável e consistente com o design system.

### Skill 5 — Data-Dense Interfaces Expert

Especialista em interfaces com grandes quantidades de informação.

Abranja:

- Dashboards.
- Tabelas complexas.
- Filtros avançados.
- Busca.
- Paginação.
- Ordenação.
- Ações em lote.
- Detalhes de registros.
- Painéis laterais.
- Indicadores e métricas.
- Gráficos.
- Estados vazios.
- Feedback de operações.

Ensine o agente a escolher a representação mais adequada para cada tipo de informação.

Evite transformar tudo em cards.

Evite dashboards visualmente bonitos, mas difíceis de interpretar.

Priorize legibilidade, escaneabilidade e eficiência operacional.

### Skill 6 — Visual Design Reviewer

Responsável pela revisão crítica das interfaces implementadas.

Sempre que houver ferramentas disponíveis, execute a aplicação e inspecione visualmente as telas.

Avalie:

- Alinhamento.
- Espaçamento.
- Hierarquia visual.
- Tipografia.
- Consistência dos componentes.
- Responsividade.
- Contraste.
- Estados interativos.
- Overflow.
- Truncamento de conteúdo.
- Acessibilidade.
- Densidade informacional.
- Consistência com o design system.

Faça revisões em diferentes tamanhos de viewport, incluindo desktop e mobile.

Identifique problemas, corrija-os e revise novamente.

Quando a inspeção visual não estiver disponível, execute uma revisão estática e declare explicitamente essa limitação.

Nunca afirme que uma tela foi validada visualmente sem realmente inspecioná-la.

## 4. Rules globais do Codex

Além das skills, crie instruções globais ou de projeto utilizando AGENTS.md e os mecanismos oficialmente suportados pelo Codex.

As regras devem estabelecer que:

1. Antes de implementar interfaces, analisar requisitos, contexto e padrões existentes.
2. Planejar a hierarquia e composição da informação.
3. Utilizar as skills especializadas conforme a natureza da tarefa.
4. Priorizar Zard UI e os tokens do projeto.
5. Evitar CSS arbitrário, duplicação e inconsistência visual.
6. Preservar acessibilidade e responsividade.
7. Evitar alterações desnecessárias em componentes compartilhados.
8. Revisar visualmente quando houver ferramentas disponíveis.
9. Não inventar APIs ou funcionalidades das bibliotecas.
10. Preservar a identidade visual existente, salvo quando a tarefa solicitar uma reformulação.

As regras devem ser concisas. O conhecimento detalhado deve permanecer nas skills e seus arquivos de referência.

Evite instruções conflitantes e carregamento desnecessário de contexto.

## 5. Workflow obrigatório de design

Toda tarefa relevante de interface deve seguir este processo:

**Etapa 1 — Discovery**

Entender a funcionalidade, os usuários, o fluxo e os requisitos.

Inspecionar telas semelhantes no projeto.

**Etapa 2 — UX Architecture**

Organizar as informações.

Definir prioridades e padrões de interação.

**Etapa 3 — Layout Planning**

Planejar a estrutura visual antes de implementar.

Determinar containers, grids, seções, espaçamentos e comportamento responsivo.

**Etapa 4 — Component Mapping**

Mapear a composição planejada para componentes reais do Zard UI.

**Etapa 5 — Implementation**

Implementar utilizando Angular, Tailwind e os padrões existentes.

**Etapa 6 — Design Review**

Revisar qualidade visual, funcionalidade, acessibilidade e responsividade.

**Etapa 7 — Refinement**

Corrigir os problemas encontrados e validar novamente.

Para alterações pequenas, simplifique o processo proporcionalmente, sem criar burocracia desnecessária.

## 6. Exemplos práticos obrigatórios

Inclua nas referências das skills exemplos de decisões reais de design.

Exemplo A: Cadastro com 40 campos.

O agente deve explicar como agrupar os campos, quando utilizar abas, como distribuir as colunas e onde posicionar as ações.

Exemplo B: Listagem com muitos filtros.

O agente deve decidir quais filtros permanecem visíveis, quais ficam em uma área avançada e como organizar tabela e ações.

Exemplo C: Dashboard administrativo.

O agente deve definir hierarquia dos indicadores, agrupamento dos gráficos e distribuição das informações.

Exemplo D: Tela de detalhes de uma entidade.

O agente deve decidir como apresentar informações gerais, histórico, relacionamentos e ações contextuais.

Esses exemplos devem demonstrar raciocínio de design, e não apenas código.

## 7. Organização e instalação

Inspecione primeiro a estrutura e as convenções do Codex disponíveis no ambiente.

Crie as skills nos diretórios corretos, com arquivos SKILL.md válidos, metadados adequados e referências organizadas.

Prefira uma arquitetura com carregamento progressivo das referências, evitando incluir toda a documentação no contexto de cada tarefa.

Defina gatilhos claros para cada skill, evitando sobreposição excessiva.

Crie também um AGENTS.md apropriado ao escopo escolhido, preservando instruções já existentes.

Não sobrescreva configurações do projeto sem analisar seu conteúdo.

## 8. Validação obrigatória

Antes de concluir:

- Validar a estrutura das skills.
- Verificar os arquivos SKILL.md.
- Confirmar caminhos e referências.
- Verificar compatibilidade com o Codex instalado.
- Revisar possíveis conflitos entre regras.
- Testar a ativação das skills com solicitações representativas.
- Confirmar que as referências técnicas ao Zard UI correspondem à documentação verificada.

Se possível, execute um teste prático criando ou melhorando uma interface isolada, sem comprometer funcionalidades existentes.

## 9. Resultado esperado

Ao final, apresente:

1. As skills criadas e suas responsabilidades.
2. As regras globais ou de projeto implementadas.
3. A estrutura de diretórios.
4. As referências utilizadas.
5. Como as skills são ativadas pelo Codex.
6. Como utilizá-las em novos projetos Angular.
7. Os testes realizados e suas limitações.
8. Sugestões de evolução do design system.

## Princípio fundamental

**Não quero uma IA que simplesmente saiba usar componentes do Zard UI. Quero uma IA que saiba projetar interfaces profissionais e utilize o Zard UI como ferramenta de implementação.**

O objetivo é obter a qualidade de composição, hierarquia visual, consistência e experiência associada a produtos modernos inspirados no shadcn/ui.

Priorize qualidade de design, decisões justificadas, reutilização e consistência.

Comece pesquisando as referências e inspecionando o ambiente. Depois, proponha a arquitetura definitiva e implemente as skills e regras, validando o resultado.

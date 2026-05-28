# projeto_trainee
Comprovação de Fluxo de Trabalho Real no GitHub Para comprovar o uso real do versionamento e da gestão do projeto, a equipe desenvolveu o modelo Git Flow (ou GitHub Flow), garantindo que nenhuma alteração seja feita sem rastreabilidade.

Passo a passo das evidências geradas:

Problemas: As tarefas foram criadas no GitHub Projects (ex: Configurar ambiente local, Criar POPs de Desenvolvimento).

Filiais: O código nunca é comitado diretamente na principal. Para cada edição, criamos uma ramificação específica (ex: feature/setup-ambiente).

Commits (Commits Convencionais): Os commits seguem um padrão semântico para facilitar o histórico (ex: feat: adicionar documentação do ambiente).

Pull Requests (PR): Após o desenvolvimento, uma filial é enviada ao repositório e um PR é aberto para o principal da filial.

Code Review: Outro membro da equipe comenta no PR ("Aprovado", "Ajustar linha X") antes de realizar o Merge, garantindo uma revisão por pares.

Procedimentos Operacionais Padrão (POPs) Função: Desenvolvedor(a) de Software POP - Versionamento de Código (Git Flow)

Objetivo: Padronizar a entrada de novo código no repositório.

Passos:

Atualizar um branch principal localmente (git pull origin development).

Criar branch a partir do issue correspondente (git checkout -b feature/nome-da-tarefa).

Desenvolver e testar o código localmente.

Fazer commit semânticos (feat:, fix:, docs:).

Fazer o push da branch (git push origin feature/nome-da-tarefa).

Abrir Pull Request (PR) assinalando pelo menos um revisor técnico.

POP - revisão de código

Objetivo: Garantir a qualidade do código antes da integração.

Passos:

O revisor deve baixar a agência do PR localmente.

Rodar o aplicativo para verificar se a funcionalidade atende aos critérios da edição.

Revise a legibilidade e arquitetura do código no GitHub.

Inserir comentários sugerindo melhorias ou aprovar o PR com o status "Aprovar".

Função: Scrum Master / Tech Lead POP - Planejamento da Sprint

Objetivo: Definir o escopo de trabalho do próximo ciclo.

Passos:

Revisar o Backlog do Produto junto com a equipe.

Selecionar as Questões Prioritárias para a Sprint.

Atribuir pontos de complexidade (Story Points) para cada tarefa.

Definir os responsáveis ​​pelas entregas.

Registrador de escopo no GitHub Projects ou ferramenta ágil equivalente.

POP - Execução de Deploy e Release

Objetivo: Padronizar a entrega da Sprint para o ambiente de produção.

Passos:

Bloquear novos PRs de recurso para lançamento de branch.

Rodar uma bateria de testes manuais e automatizados.

Fazer o merge do branch release para o main.

Gerar uma Tag de versão (ex: v1.0.0) no GitHub marcando o fim do ciclo.

Gestão de Projetos: Sprint Template Padrão de Sprint Objetivo da Sprint: [Descrever em uma frase o valor principal a ser entregue] Backlog da Sprint: [Listar os Issues definidos, seus responsáveis ​​e o status] Critérios de Pronto (DoD):

Código revisado por um par.

Funcionalidade validada nos testes locais.

Documentação atualizada (se aplicável).

Comprovação de Execução: Sprint de Setup e Infraestrutura Objetivo: Estabelecer o repositório base, a documentação de arquitetura e o ambiente de desenvolvimento local para todos os membros da equipe. Evidências de Execução:

Issue Criação do README e POPs - Status: DONE (Merge via Pull Request).

Problema Configuração de linter e formatador de código - Status: DONE (Merge via Pull Request).

Issue Criação do Kanban e template da Sprint - Status: DONE (Merge via Pull Request). Retrospectiva: A equipe conseguiu entregar a configuração inicial no prazo. Identificamos como ponto de melhoria a demora na aprovação dos PRs, então limitamos o tempo máximo de revisão de código para 24 horas no próximo ciclo.

Documentação do Ambiente de Desenvolvimento Este guia descreve as etapas necessárias para configurar o ambiente do projeto localmente.

Pré-requisitos certifique-se de ter as seguintes ferramentas instaladas:

Git

Node.js

Docker (opcional, para rodar o banco de dados)

Passo a Passo para Instalação

Clone o repositório: rode o comando git clone [url-do-repositorio].

Instale as dependências: acesse a pasta do projeto e rode npm install.

Configure como Variáveis ​​de Ambiente: faça uma cópia do arquivo de exemplo (cp .env.example .env) e preencha com as credenciais locais.

Inicie o servidor: rode o comando npm run dev. A aplicação estará disponível em http://localhost:3000 .

Referências Bibliográficas SUTHERLAND, Jeff. Scrum: a arte de fazer o dobro do trabalho na metade do tempo. Rio de Janeiro: Sextante, 2014.

CHACON, Scott; STRAUB, Ben. Pró Git. 2. ed. Nova York: Apress, 2014. Disponível em: https://git-scm.com/book/en/v2 .

ATLASSIANO. Fluxo de trabalho do Gitflow. Disponível em: https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow . Acesso em: [Dados atuais].# proj_trainee

### Tipo de Mudança

*(Marque uma ou mais opções)*

-   [ ] **Feature**: Implementa uma nova funcionalidade ou um novo recurso.
-   [ ] **Bug Fix**: Corrige um comportamento inesperado ou um erro.
-   [ ] **Refatoração**: Melhoria na estrutura ou no código, sem alterar o comportamento externo.
-   [ ] **Débito Técnico**: Endereça um problema conhecido de design, performance ou manutenibilidade.
-   [ ] **Doc**: Atualizações na documentação (READMEs, guias, etc.).
-   [ ] **Outro**: Descreva a mudança abaixo.

### O que este Pull Request faz?

*(Descreva a mudança em termos de negócio. Por que essa mudança é necessária? Qual problema ela resolve para o usuário ou para a empresa? Use a linguagem do time de produto.)*

### Como eu sei que a mudança funciona?

*(Descreva como você testou sua mudança. Qual a evidência de que a mudança alcançou seu objetivo?)*

-   [ ] Testes Unitários
-   [ ] Testes de Integração
-   [ ] Testes Manuais (inclua os passos para reproduzir)
-   [ ] A mudança foi testada em um ambiente de homologação?
-   [ ] Outros (descreva)

### Qual o impacto técnico?

*(Descreva o impacto técnico desta mudança para o sistema. É uma mudança de performance? Uma nova dependência?)*

-   **Performance**: [ ] Melhoria / [ ] Não Aplicável / [ ] Possível Degradação (justifique)
-   **Dependências**: [ ] Novas dependências adicionadas / [ ] Nenhuma alterada
-   **Segurança**: [ ] Mudança afeta a segurança de alguma forma? (justifique)
-   **Escalabilidade**: [ ] A mudança afeta a escalabilidade do serviço? (justifique)

### Pontos de atenção para o Revisor

*(Liste qualquer ponto específico que você gostaria que o revisor olhasse com atenção. Se for uma mudança complexa, ajude o revisor a entender a lógica.)*

-   `[arquivo-principal.go]`: Preste atenção na lógica de `X` na linha `Y`.
-   `[arquivo-de-configuracao.ts]`: A nova variável de ambiente `Z` foi adicionada.
-   [ ] Este PR resolve a tarefa #[número-da-tarefa]
-   [ ] Este PR contém uma refatoração grande, e eu gostaria de feedback sobre a estrutura do código.

### Checklist do Autor

-   [ ] Meu código segue o style-guide definido em [LINK_PARA_SEU_STYLE_GUIDE].
-   [ ] Meu código está bem comentado, especialmente em áreas complexas.
-   [ ] A documentação (interna e externa) foi atualizada se necessário.
-   [ ] Adicionei ou atualizei os testes para cobrir minha mudança.
-   [ ] O PR está dentro de um tamanho razoável. Se não, explique o porquê.
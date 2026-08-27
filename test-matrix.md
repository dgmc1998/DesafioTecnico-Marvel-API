# Matriz de Cenários

| ID | Cenário | Camada | Prioridade | Automatizado | Justificativa |
|----|----------|---------|------------|--------------|---------------|
| HERO-01 | Listar heróis | API | Alta | Sim | Fluxo principal da API |
| HERO-02 | Validar estrutura da resposta | API | Alta | Sim | Garante contrato |
| HERO-03 | Quantidade de registros | API | Média | Não | Valor baixo e variável |
| HERO-04 | Lista vazia | API | Média | Sim | Cenário negativo |
| HERO-05 | Tempo de resposta | API | Alta | Sim | Experiência do usuário |
| BUS-01 | Buscar por nome | API | Alta | Sim | Funcionalidade crítica |
| BUS-02 | Buscar por trecho | API | Média | Sim | Busca parcial |
| BUS-03 | Buscar inexistente | API | Alta | Sim | Validação negativa |
| BUS-04 | Campo vazio | API | Média | Sim | Regra funcional |
| BUS-05 | Caracteres especiais | API | Média | Não | Baixa criticidade |
| DET-01 | Detalhes do herói | API | Alta | Sim | Fluxo principal |
| DET-02 | Validar atributos | API | Alta | Sim | Integridade dos dados |
| DET-03 | Herói inexistente | API | Média | Sim | Tratamento de erro |
| DET-04 | Campos nulos | API | Baixa | Não | Dependente dos dados |
| DET-05 | Estrutura do detalhe | API | Alta | Sim | Contrato |
| UI-01 | Carregar página | UI | Alta | Sim | Jornada inicial |
| UI-02 | Exibir lista | UI | Alta | Sim | Conteúdo principal |
| UI-03 | Abrir detalhes | UI | Alta | Sim | Navegação crítica |
| UI-04 | Busca no frontend | UI | Alta | Sim | Fluxo principal |
| UI-05 | Renderizar imagens | UI | Média | Sim | Experiência visual |
| UI-06 | Responsividade | UI | Baixa | Não | Alto custo |
| UI-07 | Acessibilidade básica | UI | Média | Sim | Boa prática |
| UI-08 | Falha de carregamento | UI | Baixa | Não | Necessita mock |
| TRV-01 | Loading | UI | Média | Não | Instável |
| TRV-02 | Erro da API | Integração | Média | Não | Requer interceptação |
| TRV-03 | Timeout | Integração | Baixa | Não | Ambiente controlado |
| TRV-04 | Múltiplos cliques | UI | Baixa | Não | Baixo risco |
| TRV-05 | Console sem erros | UI | Média | Sim | Qualidade técnica |
| TRV-06 | API indisponível | Integração | Baixa | Não | Necessita mock |

# Plano de Testes – Marvel Rivals QA Challenge

## 1. Objetivo

Validar a qualidade da aplicação Marvel Rivals Hub, considerando a integração entre o frontend público e a Marvel Rivals API, garantindo que os dados sejam exibidos corretamente e que os fluxos críticos do usuário funcionem conforme esperado.

---

## 2. Escopo

### Em escopo

**API**
- Listagem de heróis
- Busca de heróis
- Detalhes do herói
- Estrutura das respostas
- Performance básica

**Frontend**
- Carregamento da página
- Exibição da lista de heróis
- Busca por nome
- Navegação para detalhes
- Renderização de imagens
- Acessibilidade básica

### Fora do escopo

- Testes de carga
- Testes de segurança
- Compatibilidade entre múltiplos navegadores
- Responsividade avançada
- Testes mobile nativos

---

## 3. Riscos Identificados

| Risco | Impacto | Mitigação |
|--------|---------|-----------|
| API indisponível | Alto | Validação de códigos HTTP e tratamento de erro |
| Estrutura JSON alterada | Alto | Testes de contrato |
| Busca retornar dados incorretos | Alto | Testes positivos e negativos |
| Lentidão da API | Médio | Validação de tempo de resposta |
| Imagens não carregarem | Médio | Testes de renderização no frontend |

---

## 4. Estratégia de Testes

Foi adotada uma estratégia em camadas para reduzir custo de manutenção e aumentar confiabilidade.

### Camada API

Objetivo:
- Validar regras de negócio
- Contrato da API
- Dados retornados
- Performance

Ferramenta:
- Robot Framework
- RequestsLibrary

### Camada UI

Objetivo:
- Validar jornada crítica do usuário
- Garantir integração visual com a API

Ferramenta:
- Robot Framework
- Browser Library

---

## 5. Critérios de Priorização

Os cenários foram classificados conforme:

| Prioridade | Critério |
|------------|----------|
| Alta | Fluxos essenciais do usuário |
| Média | Funcionalidades importantes, porém secundárias |
| Baixa | Cenários de alto custo ou baixo risco |

---

## 6. Critérios de Entrada

- API disponível
- Frontend acessível
- Ambiente configurado
- Dependências instaladas

---

## 7. Critérios de Saída

A execução será considerada satisfatória quando:

- Todos os testes críticos forem executados
- Não houver falhas bloqueantes
- Evidências forem geradas
- Relatórios HTML forem produzidos

---

## 8. Ferramentas Utilizadas

- Robot Framework
- Browser Library
- RequestsLibrary
- Python 3.12
- GitHub

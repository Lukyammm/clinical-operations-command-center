# Glossário e padrão de linguagem — SIGEP-HUC

Objetivo: garantir linguagem única, em português operacional, na interface do
sistema. Termos técnicos/de desenvolvedor **não** devem aparecer para o usuário
final — ficam restritos ao código.

## Princípios

- Rótulos visíveis sempre em **português**, sem mistura com inglês.
- Verbos de ação no infinitivo: "Cadastrar", "Lançar dados", "Editar", "Excluir".
- Evitar jargão interno (nomes de função, status técnicos) na tela.

## Termos canônicos (rótulo visível)

| Conceito | Rótulo correto na tela | Evitar |
|----------|------------------------|--------|
| Visão consolidada inicial | **Painel executivo** | "Dashboard" |
| Carregar/abrir um registro | **Abrir** / **Ver detalhes** | "load", "open drawer" |
| Lançar resultados do mês | **Lançar dados** / **Lançamento mensal** | "fix data", "input" |
| Conferir e corrigir dados | **Revisar dados** | "review date", "data review" |
| Aplicar correção sugerida | **Aplicar correção** | "applySuggestion" |
| Aplicar várias correções | **Aplicar correções em lote** | "applySuggestionBatch" |
| Corrigir manualmente | **Corrigir manualmente** | "fixDataManually" |
| Etapa de análise do processo | **Em análise** | "In Analysis" |
| Higienização de dados | **Limpeza de dados** | "Cleanup" |
| Foto/registro do período | **Registro do período** | "Snapshot" |
| Gestor responsável | **Gestor** | "Manager" |
| Carregando conteúdo | **Carregando…** | "Loading…" |

## Nomes internos (NÃO aparecem na interface)

Os identificadores abaixo são **internos** (funções/estados em `Index.html` e
`Code.gs`) e não são exibidos ao usuário. Devem ser renomeados apenas em uma
refatoração planejada — sem impacto de UX imediato e com risco de regressão se
feitos de forma avulsa:

`renderDashboard`, `loadAdminData`, `applySuggestion`, `applySuggestionBatch`,
`fixDataManually`, `refreshDashboardFromLocal`.

> Diretriz: ao criar **novos** rótulos visíveis, consulte este glossário. Ao
> renomear nomes internos, fazê-lo em PR dedicado, garantindo que nenhuma string
> técnica vaze para a tela.
</content>
</invoke>

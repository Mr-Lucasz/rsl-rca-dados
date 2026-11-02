# Dados da RSL — Análise de Causa Raiz (RCA) na Qualidade de Software

Conjunto de dados de apoio ao preprint:
Rodrigues, L. (2026). *Análise de Causa Raiz na Qualidade de Software: uma Revisão Sistemática da Literatura*. Preprint.

Autor: Lucas Rodrigues (ORCID 0009-0006-5026-5412) — l.cunha14.lc@gmail.com
Licença: CC BY 4.0

Revisão de literatura: não há dados primários de participantes humanos. Os PDFs dos estudos primários não são redistribuídos (direitos autorais); cada estudo é identificado por DOI/URL.

## Estrutura

| Pasta/arquivo | Etapa | Registros |
|---|---|---:|
| `01_buscas/acm_2010_2025.csv` | Exportação ACM Digital Library (2010–2025) | 401 |
| `01_buscas/springer_2010_2025.csv` | Exportação SpringerLink (2010–2025) | 114 |
| `01_buscas/ieee_2010_2025.csv` | Exportação IEEE Xplore (2010–2025) | 13 |
| `01_buscas/scopus.csv` | Exportação Scopus (API, visão padrão) | 14 |
| `02_triagem/duplicates_removed.csv` | Duplicatas removidas | — |
| `02_triagem/screening_candidates.csv` | Registros para triagem título/resumo | 529 |
| `02_triagem/title_abstract_included.csv`, `title_abstract_maybe.csv` | Aprovados/dúvida na triagem título/resumo | 49 + 28 |
| `02_triagem/full_text_candidates.csv` | Candidatos à leitura em texto completo | 77 |
| `02_triagem/full_text_excluded.csv` | Excluídos em texto completo, com motivo (CE) | 25 |
| `02_triagem/full_text_included.csv` | Elegíveis antes da consolidação de duplicata | 52 |
| `02_triagem/prisma_counts.json` | Contagens do fluxo PRISMA | — |
| `03_extracao/extracao_51_estudos.csv` | Extração final (RQ1–RQ6) do corpus de 51 estudos | 51 |

## Extração (`03_extracao/extracao_51_estudos.csv`)

- `id`: identificador do protocolo de extração; `ref_manuscrito`: chave da referência no preprint (`rslNN`).
- Colunas analíticas: `contexto_RQ1`, `tecnica_RCA_RQ2`, `automacao_RQ3`, `beneficios_RQ4`, `desafios_RQ5`, `lacunas_RQ6`.
- Consolidação de duplicata: o registro `id=38` (Pacheco, 2011, CACM, DOI 10.1145/2043174.2043189) foi removido por ser republicação de `id=30` (ACM Queue, DOI 10.1145/2039359.2039361, `rsl22`), reduzindo 52 → 51 estudos.

## Período das buscas

16 a 18 de junho de 2026; estudos publicados entre 2010 e 2025.

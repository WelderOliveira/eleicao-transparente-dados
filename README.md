# Eleição Transparente — dados

JSONs estáticos gerados a partir da prestação de contas eleitorais 2026 do TSE
(candidatos), servidos via GitHub Pages para o dashboard.

Fonte: https://dadosabertos.tse.jus.br/dataset/prestacao-de-contas-eleitorais-2026 (CC-BY).
Os dados são parciais e mudam a cada nova versão publicada pelo TSE (veja `source_date`).

| Arquivo | Conteúdo |
|---|---|
| `macro_brasil.json` | Totais nacionais, fontes de recurso, gasto por partido e por macro-categoria |
| `search_index.json` | `[{i, n, p, c, u}]` — id, nome de urna, partido, cargo, UF |
| `candidatos/<id>.json` | Contas de um candidato (`candidate.*`) |

Base URL: `https://welderoliveira.github.io/eleicao-transparente-dados/`

Gerado por `etl/build_json.py` (projeto local `tse`).

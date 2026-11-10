# Grafos e ciência de redes no Order Batching Problem: material suplementar

Material suplementar do mapeamento sistemático da literatura *O Estado da Arte do Order Batching Problem com Grafos e Ciência de Redes*.

## Arquivos

| Arquivo | Conteúdo |
|---|---|
| `consulta_scopus.txt` | Consulta exata executada na Scopus, com data e número de registros |
| `triagem_110_registros.csv` | Os 110 registros recuperados, com a *string* de origem, a decisão (selecionado, rejeitado ou duplicata), o critério aplicado e o estrato |
| `avaliacao_qualidade.csv` | Notas por critério (QA1 a QA5) dos estudos com texto completo e situação dos demais |

Os arquivos CSV usam `;` como separador e codificação UTF-8. A planilha de triagem traz apenas dados bibliográficos (título, autores, ano, veículo e DOI); os resumos não são redistribuídos, conforme os termos de uso da Scopus.

## Critérios de seleção

Um registro foi selecionado quando atendeu a pelo menos um critério de inclusão e a nenhum de exclusão.

| Código | Critério |
|---|---|
| CI-01 | Trata agrupamento de pedidos, formação de ondas ou seleção de corredores em armazéns |
| CI-02 | Modela a afinidade entre pedidos ou itens de um armazém por grafos, hipergrafos ou análise de redes |
| CI-03 | (S4 e S5) Resolve outro problema combinatório com objetivo de razão em grafos ou com a topologia como guia da busca |
| CE-01 | *Batching* em aprendizado profundo ou *scheduling* de máquinas |
| CE-02 | Grafo usado apenas para representar o *layout* e calcular caminhos mínimos |
| CE-03 | Duplicata, resumo estendido, volume de anais sem estudo primário ou texto fora do inglês, português ou espanhol |
| CE-04 | (S4 e S5) Comunidades ou centralidade como o próprio objetivo; agrupamento capacitado sem objetivo de razão nem uso da topologia; ou restrições específicas que impedem a transferência |
| NC | Não atende a nenhum critério de inclusão |

## Avaliação de qualidade

Cada critério recebe 1 (atende), 0,5 (atende parcialmente) ou 0 (não atende). Estudos com nota total inferior a 2,5 têm os resultados desconsiderados na síntese.

| Código | Pergunta |
|---|---|
| QA1 | O problema e o objetivo são definidos de forma clara, com formulação ou definição formal? |
| QA2 | O método, incluindo o papel do grafo, é descrito com detalhe suficiente para ser reproduzido? |
| QA3 | A avaliação usa instâncias identificadas (*benchmark* público ou geração descrita)? |
| QA4 | Os resultados são comparados com métodos de referência, limites ou soluções ótimas, com análise estatística quando há aleatoriedade? |
| QA5 | As limitações são discutidas ou o código e os dados são disponibilizados? |

## Resumo da seleção

110 registros recuperados, 1 duplicata, 82 rejeitados (NC 25; CE-02 2; CE-03 8; CE-04 47) e 27 selecionados: 1 no núcleo, 13 de contexto e 13 transferíveis.

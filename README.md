# Processamento e Visualização de Acórdãos Jurídicos: Uma Abordagem Baseada em NLP e Business Intelligence

[![UFG](https://upload.wikimedia.org/wikipedia/commons/7/79/Marca_da_UFG.png)]()

**Universidade Federal de Goiás**
Instituto de Informática
Pós Graduação em Banco de Dados Para Big Data

**Autores:** Guilherme Barbosa Gomes, Vitor Augusto Dib Martinho

**Orientador:** Prof. Dr. Márcio de Souza Dias

**Goiânia, 2025**

## Resumo do Projeto

Este projeto apresenta uma abordagem para o **processamento e visualização de um grande volume de acórdãos jurídicos** do Superior Tribunal de Justiça (STJ) utilizando **Processamento de Linguagem Natural (NLP)** e **Business Intelligence (BI)** [1]. O objetivo principal é facilitar a análise e a extração de insights a partir desses documentos textuais, que se tornam cada vez mais numerosos com a digitalização do sistema judiciário brasileiro [1, 2].

Foi desenvolvido um *pipeline* em **Python** para extrair, tratar e estruturar dados textuais dos acórdãos [1, 3]. As técnicas de NLP, implementadas com a biblioteca **spaCy** (utilizando o modelo `pt_core_news_lg`), incluíram pré-processamento textual, identificação de entidades nomeadas e extração de métricas linguísticas [1]. Um subconjunto de **10 mil documentos** de um *corpus* maior de dois milhões foi analisado [1].

Os dados extraídos foram então estruturados e visualizados em um **painel interativo no Power BI** [1, 4]. Este painel permite aos usuários explorar informações como a frequência de termos jurídicos, a distribuição geográfica dos processos, entidades recorrentes (pessoas, organizações, locais, leis) e a densidade lexical dos textos [1, 5].

Os resultados demonstram a **viabilidade da integração de NLP e BI na exploração de dados jurídicos**, oferecendo suporte à tomada de decisões e à pesquisa acadêmica no campo do Direito [1, 6].

## Palavras-chave

Processamento de Linguagem Natural, Acórdãos, Business Intelligence, Visualização de Dados, Direito Digital, Legal Analytics [7, 8].

## Estrutura do Trabalho

O projeto foi estruturado nas seguintes etapas principais:

*   **Coleta e Preparação dos Dados:** Acórdãos jurídicos em formato `.txt` foram coletados de repositórios públicos [9].
*   **Pré-processamento Textual:** Utilização de bibliotecas Python como `re`, `pandas`, `spaCy` e `collections` para limpeza, tokenização, lematização, contagem de termos e reconhecimento de entidades nomeadas [3, 10].
*   **Estruturação e Modelagem dos Dados:** Os dados processados foram organizados em `DataFrames` para facilitar a exportação e manipulação no Power BI [11].
*   **Construção do Dashboard:** Desenvolvimento de um painel interativo no Power BI com visualizações dinâmicas para explorar os dados extraídos [1, 12]. O modelo de dados no Power BI utilizou um esquema de *Star-Schema Híbrido* com tabelas fato (e.g., `Fact_Resumo`, `Fact_Palavras_Chave`, `Fact_Pessoas`) e uma tabela dimensional (`Dim_Arquivos`) [13, 14].
*   **Validação e Testes:** Verificação da consistência dos dados e do funcionamento dos filtros e interações no Power BI [15].

## Tecnologias Utilizadas

*   **Python:** Linguagem de programação utilizada para o processamento de linguagem natural e manipulação de dados [3, 16].
    *   **spaCy:** Biblioteca para NLP, utilizada para tokenização, lematização e reconhecimento de entidades nomeadas [1, 3, 17].
    *   **pandas:** Biblioteca para manipulação e análise de dados tabulares [3, 17].
    *   **collections (Counter):** Para contagem de frequência de palavras e termos [3, 17, 18].
    *   **re (expressões regulares):** Para padronização e limpeza textual [3, 17, 19].
*   **Microsoft Power BI:** Ferramenta de Business Intelligence utilizada para a criação do dashboard interativo e visualização dos dados [1, 4, 13].

## Principais Resultados e Insights

O dashboard no Power BI permitiu obter diversos *insights* sobre os acórdãos analisados [20]:

*   **Volume e Complexidade Textual:** Análise do número de documentos, caracteres, palavras, sentenças e densidade lexical [21].
*   **Palavras-Chave e Temas Dominantes:** Identificação dos termos mais frequentes, como "Recurso", "Especial" e "Agravo", indicando os temas centrais dos acórdãos [22].
*   **Entidades Mais Citadas:** Extração e análise da frequência de organizações (e.g., "Tribunal de Justiça", "Superior Tribunal de Justiça"), pessoas, leis (e.g., "8137/90", "8429/92") e locais mencionados nos documentos [23].
*   **Distribuição Geográfica:** Visualização da distribuição dos acórdãos por estado brasileiro, com maior concentração em SP, RJ, DF e RS [24].
*   **Estrutura Gramatical:** Análise da predominância de substantivos em relação a verbos e adjetivos, consistente com a natureza formal dos textos jurídicos [24].

## Possibilidades de Análise

O dashboard oferece uma ampla gama de análises, permitindo ao usuário [20]:

*   Avaliar a complexidade e extensão dos documentos jurídicos.
*   Medir a densidade linguística do *corpus*.
*   Identificar os principais temas e termos jurídicos recorrentes.
*   Visualizar a estrutura gramatical predominante nos textos.
*   Investigar a frequência e o tipo de entidades mencionadas.
*   Comparar a origem geográfica dos acórdãos por estado.
*   Explorar padrões e tendências para estudos jurídicos, decisões estratégicas ou pesquisa acadêmica.

## Trabalhos Futuros

Para trabalhos futuros, recomenda-se [25]:

*   Expansão da base de dados de acórdãos.
*   Utilização de modelos linguísticos mais avançados, como *transformers*.
*   Inclusão de métricas qualitativas, como análise de sentimentos e detecção de similaridade entre acórdãos.

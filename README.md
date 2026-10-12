# Hotspot mapping and prioritization of railway accidents via DBSCAN: application to Rumo Malha Sul
# Mapeamento e priorização de hotspots de sinistros ferroviários via DBSCAN: aplicação na Rumo Malha Sul

## English


**Authors:** Aluisio Guilherme Regazzo; Guilherme Benitez Frehse; Lucas Gabriel Souza da Silva; Suzane dos Santos

**Description.** The notebook downloads railway occurrence records from the ANTT Open Data Portal (Brazil), audits and standardizes the data, restricts it to 2021–2025, and applies DBSCAN (using only `Linha + Quilômetro_Inicial`, i.e., line + kilometer position) to Rumo Malha Sul (RMS) occurrences. It then computes a Severity Score, tests sensitivity to hyperparameters and score weights

**Files**
- `hotspots_ferroviarios_dbscan_RMS_2021_2025.ipynb` – full notebook (data acquisition → modeling → figures/table), with saved outputs
- `requirements.txt` – library versions
- `README.md` – this file

**How to run.** Python 3.10+ (run with 3.13); `pip install -r requirements.txt`; open Jupyter and *Run All*. Internet access is required.

**Data.** Not redistributed here. The notebook downloads it directly from the ANTT Open Data Portal (https://dados.antt.gov.br), CKAN resource `b3851bf8-9c4c-4452-93f6-ddaba3992e60`, via the `datastore_search` API. The resource covers Dec/2020–Jan/2026; only 2021–2025 is analyzed. Data accessed on September 2026. Because ANTT may update the base, results may differ if re-run later.

**Environment.** Python 3.13.16, pandas 2.2.3, NumPy 2.1.3, scikit-learn 1.6.1, SciPy 1.16.3, Matplotlib 3.10.0. DBSCAN is deterministic (no random seeds).

**License.** Code:  CC BY 4.0. Source data remain under ANTT's open data terms.




## Português


**Descrição.** O notebook baixa os registros de ocorrências ferroviárias do Portal de Dados Abertos da ANTT, audita e padroniza a base, recorta 2021–2025 e aplica o DBSCAN (apenas sobre `Linha + Quilômetro_Inicial`) às ocorrências da Rumo Malha Sul (RMS). Depois calcula o Score de Severidade, testa a sensibilidade dos hiperparâmetros e dos pesos e gera as figuras e a tabela do estudo.

**Como executar.** Python 3.10+; `pip install -r requirements.txt`; abrir o Jupyter e executar todas as células. É necessário acesso à internet.

**Dados.** Não são redistribuídos aqui; o notebook os obtém diretamente da API da ANTT (recurso `b3851bf8-9c4c-4452-93f6-ddaba3992e60`). Acesso em: Setembro de 2026. A base pode ser atualizada pela ANTT, então a reexecução futura pode gerar resultados diferentes.

**Licença.** Código: CC BY 4.0. Os dados de origem seguem os termos de dados abertos da ANTT.

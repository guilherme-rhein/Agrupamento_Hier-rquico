<img src="https://raw.githubusercontent.com/guilherme-rhein/Agrupamento_Hierarquico/main/img/ebac_data_science.png" alt="Ebac,Data Science">
<h1 align="center">
    💫 Hierarchical Clustering 💫</a>
</h1>

<p align="center"> O objetivo deste projeto é poder gerar insights valiosos, partindo da seleção das principais variáveis que definam o comportamento de navegação e informações temporais dos usuários referentes as sessões de acesso ao portal, analisando e buscando por padrões nos grupos do modelo. </p>

---

<h3 align="center">
    ▶️ Acesse o Projeto Aqui: <a href="">Aplicativo para Segmentação de Clientes ▶️</a>
    <br>
</h3>

---

## Agrupamento Hierarquico dos clientes 📌
Neste projeto foi utilizada a base [online shoppers purchase intention](https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset) de Sakar, C.O., Polat, S.O., Katircioglu, M. et al. Neural Comput & Applic (2018). [Web Link](https://doi.org/10.1007/s00521-018-3523-0). A base trata de registros de 12.330 sessões de acesso a páginas, cada sessão sendo de um único usuário em um período de 12 meses.<br>

Com as informações disponíveis, surge a dúvida:
>> ***"Será que clientes com comportamento de navegação diferentes possuem propensão a compra diferente?"***

## Índice ✔️

```bash
- O Projeto
- Análise Descritiva
- Seleção de Variáveis de para Agrupamento
- Agrupamentos Hierárquicos
- Analisando os Grupos 3 e 4
- Conclusão
```

## Bibliotecas Utilizadas 📚

```bash
import streamlit as st
import io

import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np

from scipy.spatial.distance  import squareform
from scipy.cluster.hierarchy import linkage
from scipy.cluster.hierarchy import dendrogram
from scipy.cluster.hierarchy import fcluster
from gower import gower_matrix
```


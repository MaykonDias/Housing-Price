#  Previsão de Preços de Imóveis ([Housing Prices](https://www.kaggle.com/datasets/yasserh/housing-prices-dataset))

Objetivo principal do projeto é predição dos valores dos imóveis usando modelo de Regressão Linear.

---

### Dicionário de variáveis

| Coluna | Tipo | Descrição |
|---|---|---|
| `price` | int64 | Preço do imóvel (target) |
| `area` | int64 | Área do terreno/construção |
| `bedrooms` | int64 | Número de quartos |
| `bathrooms` | int64 | Número de banheiros |
| `stories` | int64 | Número de andares |
| `mainroad` | object | Se está em via principal (yes/no) |
| `guestroom` | object | Possui quarto de hóspedes (yes/no) |
| `basement` | object | Possui porão (yes/no) |
| `hotwaterheating` | object | Possui aquecimento de água (yes/no) |
| `airconditioning` | object | Possui ar-condicionado (yes/no) |
| `parking` | int64 | Número de vagas |
| `prefarea` | object | Está em área preferencial (yes/no) |
| `furnishingstatus` | object | Mobília: furnished / semi-furnished / unfurnished |

---
### Análise estatístico 
Análise dos resultados percebemos que o Erro médio absoluto(MAE) tem uma margem de erro de $970043.40, que impacta negativamente no modelo. A Raiz do Erro Quadrático Médio(RMSE) de $1324506.96 que demonstra que foi um valor muito alto em comparação ao MAE demonstra presenças de outliers. O Erro Percentual Absoluto Médio(MAPE) tem um porcentagem de erro 21,04% do valores. O coeficiente R² indica que 0.6529 ou 65,29% dos explica a variância dos dados enquanto e os restante dos dados.

| Métrica | Valor |
| :--- | :---: |
| **MAE** | $ 970.043,40 |
| **RMSE** | $ 1.324.506,96 |
| **MAPE** | 21,04% |
| **R²** | 0,6529 |

O gráfico demonstra que grande parte dos dados ficam proximos a reta de inclinação, contudo, alguns dados fica bem distante assim demosntrando outliers como vimos a partir da análise do RMSE.
<img width="1001" height="699" alt="image" src="https://github.com/user-attachments/assets/6786dfc7-01fc-45fd-9dd8-e94587596116" />

---

### Conclusão
A partir das métricas estátistica do modelo, podemos perceber que a precisão esta bem abaixo do esperado. Percebi que alguns imoveis teve um valor muito elevados dos demais dados. Com isto concluo que inserir mais dados para melhoria do modelo.

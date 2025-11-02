# 📉 Análise Exploratória

## Índice

- [📓 Sobre](#-sobre)
- [🚀 Tecnologias](#-tecnologias)
- [✨ Funcionalidades](#-funcionalidades)
- [⚙️ Instalação](#-instalação)
- [⏰ Processamento Agendado (GitHub Actions)](#-processamento-agendado-github-actions)

</br>

## 📓 Sobre

Como parte do requisito mínimo de Ciência de Dados, foi desenvolvida uma análise de dados sem predição por meio das bibliotecas matplotlib e seaborn, via Python. Fonte de Dados (planilha original – recebida fábrica): Análises FFO (2).xlsx O começo do desenvolvimento da demanda foi marcado pela obtenção de dados da Fábrica de Amparo, contando com inspeções de três índices REAIS utilizados.

</br>

## 🚀 Tecnologias

As principais tecnologias e bibliotecas utilizadas neste projeto são:

* **Python 3.11**
* **pandas**
* **matplotlib**
* **seaborn**
* **threading/multithreading**

</br>

## ✨ Funcionalidades

Leitura e tratamento de dados:
- Separação por produto (FP, FV, Óleo) e seus índices.
- Tratamento de valores ausentes (NaN) e ajuste específico para setembro (apenas um dia de dados).
- Uso de dicionários para organizar dados brutos e totais.
Análise visual (funções):
 - Histogramas (gerador_histograma): identificação de padrões e repetições mensais.
    - Óleo: dados tendenciosos ao zero.
    - FP: dados padronizados e próximos.
    - FV: dados com maiores índices registrados.
 - Boxplots (gerador_boxplot): detecção de valores fora do padrão.
    - Óleo: padrão consistente até julho.
    - FP: valores extremamente consistentes.
    - FV: mudanças no padrão até junho.
Otimização
  - Multithreading para acelerar a leitura e plotagem dos dados.
  - Conversão de dataframes para formato vertical (melt) para compatibilidade com seaborn.


</br>

## ⚙️ Instalação

É necessário ter o Python (versão 3.10+).

```bash
# clonar o repositório
git clone [https://github.com/Systems-Kronos/kronos-analise-exploratoria.git](https://github.com/Systems-Kronos/kronos-analise-exploratoria.git)

# entrar no diretório
cd kronos-analise-exploratoria

# instalar dependências
pip install -r requirements.txt
````

</br>

## ⏰ Processamento Agendado (GitHub Actions)

Por se tratarem de dados estáticos (a partir de um excel obtido pela fábrica), a pipeline de atualização não é necessária.

</br>

## 📄 Licença

Este projeto está licenciado sob a licença MIT — veja o arquivo [LICENSE](https://www.google.com/search?q=LICENSE) para mais detalhes.

</br>

## 💻 Autores

  - [Júlia Penna](https://github.com/juliaPnMt1304)



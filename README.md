
![Predictive Modeling in Electronic Health Records](https://user-images.githubusercontent.com/91201232/134506117-74e637f6-c600-4405-a86f-b71800f6e4ce.png)
<br>
<br>

## Índice
- [Problema](#problema)
- [Dados](#dados)
- [Etapas](#etapas)
- [Progresso](#progresso)
- [Criador](#criador)
<br>

## Problema

O objetivo deste projeto foi prever se um paciente poderá ser readmitido em uma clínica no período de 30 dias após alta. Para isso, foi feito a construção de diversos modelos preditivos usando registros eletrônicos de saúde de uma clínica fictícia.

Esse projeto teve como base uma pesquisa realizada em 2018, chamada:

Using Electronic Health Records and Machine Learning to Make Medical-Related Predictions from Non-Medical Data

https://ieeexplore.ieee.org/document/8614004

### Registros Eletrônicos de Saúde (Electronic Health Records)

Um Registro Eletrônico de Saúde (Electronic Health Records - EHR) é uma versão digital da ficha de papel de um paciente. Os EHRs são registros em tempo real, centrados no paciente, que tornam as informações disponíveis instantânea e seguramente para usuários autorizados. Embora um EHR contenha os históricos médicos e de tratamento dos pacientes, um sistema de EHR é construído para ir além dos dados clínicos coletados no consultório de um prestador de serviços e pode incluir uma visão mais ampla do atendimento de um paciente. Os EHRs são uma parte vital da TI em saúde e podem:

- Conter o histórico médico do paciente, diagnósticos, medicamentos, planos de tratamento, datas de imunização, alergias, imagens de radiologia e resultados laboratoriais e de testes.

- Permitir acesso a ferramentas baseadas em evidências que os provedores podem usar para tomar decisões sobre o atendimento de um paciente.

- Automatiza e simplifica o fluxo de trabalho do provedor.

Um dos principais recursos de um EHR é que as informações de saúde podem ser criadas e gerenciadas por provedores autorizados em um formato digital capaz de ser compartilhado com outros provedores em mais de uma organização de saúde. Os EHRs são construídos para compartilhar informações com outros prestadores de cuidados de saúde e organizações - como laboratórios, especialistas, instalações de imagens médicas, farmácias, instalações de emergência e clínicas de escolas e locais de trabalho - para que eles contenham informações de todos os clínicos envolvidos no atendimento de um paciente.
<br>
<br>

## Dados

Para prever se um paciente poderá ser readmitido em uma clínica no período de 30 dias após alta, foi feito a construção de diversos modelos preditivos usando registros eletrônicos de saúde de uma clínica fictícia.

### Arquivos

Estão localizados no diretório `dados`

- dataset.csv - Registros eletrônicos de saúde

### Dicionário do Dados

- IDADE - Idade do paciente (variável numérica)
- SEXO_F - paciente do sexo feminino (variável categórica)
- SEXO_M - paciente do sexo masculino (variável categórica)
- ADM_CORRENTE_DIAS - Dias desde a admissão atual (variável numérica)
- RECEB_MEDICAMENTOS - Recebeu medicamentos na última internação (variável categórica)
- FEZ_EXAMES - Fez exames na última internação (variável categórica)
- DEPEND_QUIMICO - Dependendo químico (variável categórica)
- FUMANTE - Fumante (variável categórica)
- ALCOOLISMO - Alcoolismo (variável categórica)
- NUM_DIAS_INT_PREVIA - Número de internações anteriores (variável numérica)
- ADM_PREVIA_DIAS - Dias da admissão anterior (variável numérica)
- NUM_DIAS_LIC_MEDICA - Licença médica (variável numérica)
- READMISSAO_30_DIAS - Readmissão dentro de 30 dias após a alta. Variável target. 0 - Não / 1 - Sim
<br>

## Etapas

- [x] Importação e Identificação do Dados
- [x] Análise Exploratória
- [x] Construção dos Modelos Preditivos
- [x] Deploy do Modelo
- [x] Ferramentas Utilizadas
<br>

## Progresso
### Importação e Identificação do Dados
- Importação dos pacotes e bibliotecas
- Carregamento dos dados
- Entendimento do projeto

### Análise Exploratória
- Verificando se tem valores ausentes
- Função para visualizar a distribuição de cada variável
- Checando Outliers
- Correlação e Associação
- Função para calcular a associação entre variáveis categóricas
- Pré-Processamento

### Construção dos Modelos Preditivos
- Definição dos cinco melhores modelos Preditivos dado o problema de previsão se paciente será readmitido na clínica em até 30 dias após a alta:

  - Regressão Logística
  - RandomForest
  - Naive Bayes 
    - Modelo MultinomialNB
    - Modelo BernoulliNB
    - Modelo GaussianNB
  - KNN
  - Deep Learning
  
- Realização de Cross Validation nos dados usando 'K-Folds Cross Validation'
- Otimização de Hiperparâmetros usando 'Grid Search'
- Comparação de performance dos algoritmos de Machine Learning
- Preparação da Versão Final do Modelo

### Deploy do Modelo
- Entrada com dados de um novo paciente
- Ajuste do shape dos dados para o modelo
- Realização da previsão deste novo paciente 

### Ferramentas Utilizadas

- Numpy
- Scipy
- SMOTE
- Keras
- pickle
- Pandas
- Seaborn
- Sklearn
- XGBoost
- Matplotlib
- Tensorflow
- Scikitplot
- GaussianNB
- BernoulliNB
- MultinomialNB
- LogisticRegression
- KNeighborsClassifier
- RandomForestClassifier
<br>

## Criador

**Izabella Souza**

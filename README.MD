# **GreenWay: Predição de Locais para Implantação de Bikes e Patinetes**

## **Descrição do Problema**
A mobilidade urbana é um desafio crescente, especialmente em grandes cidades como São Paulo. Problemas como congestionamentos, emissão de carbono e limitações no transporte público reforçam a necessidade de alternativas sustentáveis. O **GreenWay** é um sistema que utiliza inteligência artificial para identificar regiões que necessitam de bicicletas e patinetes compartilhados, otimizando recursos e melhorando a locomoção da população.

---

## **O Sistema GreenWay**
O sistema utiliza dados reais da pesquisa Origem-Destino de São Paulo para treinar uma IA que prevê áreas de alta demanda para bikes e patinetes. Essa solução visa:

- **Sustentabilidade**: Reduzir a dependência de veículos tradicionais.
- **Eficiência**: Direcionar investimentos para regiões de maior impacto.
- **Melhoria da Experiência do Usuário**: Fornecer uma solução de transporte mais prática e integrada ao aplicativo **GreenWay**.

---

## **Metodologia**
1. **Coleta e Preparação de Dados**:
   - Dataset: Origem-Destino São Paulo 2017.
   - Colunas Selecionadas: 
     - `ZONA`: Zona do domicílio.
     - `MUNI_DOM`: Município do domicílio.
     - `TOT_VIAG`: Total de viagens realizadas pela pessoa.
     - `N_VIAG`: Número de viagens registradas.
     - `DURACAO`: Duração média das viagens (em minutos).

2. **Criação de Features**:
   - Criamos uma coluna `target`, indicando a necessidade de bikes/patinetes com base na densidade de viagens e duração média.

3. **Análise Exploratória**:
   - Visualização de padrões de viagens e identificação de regiões críticas.

4. **Modelagem**:
   - Modelo Utilizado: RandomForestClassifier.
   - Divisão dos Dados: 70% Treino e 30% Teste.
   - Métricas de Avaliação:
     - Acurácia: 100%.

---

## **Resultados**
- O modelo identificou com sucesso as regiões prioritárias para implantação.
- Dados de saída podem ser integrados ao aplicativo **GreenWay**, permitindo a visualização de mapas de calor com recomendações.

---

## **Como Usar**
1. **Entrada**: Forneça dados com as colunas `ZONA`, `MUNI_DOM`, `TOT_VIAG`, `N_VIAG`, e `DURACAO`.
2. **Saída**: Previsão binária:
   - `1`: Alta necessidade de bikes/patinetes.
   - `0`: Baixa necessidade.

---

## **Benefícios**
- **Sustentabilidade**: Promove alternativas ecológicas.
- **Otimização de Recursos**: Garante investimentos estratégicos.
- **Acessibilidade**: Facilita a locomoção da população.

---
Devs:
- Livia Mariana Lopes
- Celeste Mayumi
- Luana Vieria 


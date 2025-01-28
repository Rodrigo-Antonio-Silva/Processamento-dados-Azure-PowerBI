# Processamento-dados-Azure-PowerBI
Este projeto é um desafio do Bootcamp da Dio Suzano. Ele consistiu em integrar uma base de dados MySQL hospedada no Azure ao Power BI, realizando transformações de dados e análises, seguindo diretrizes específicas para limpeza e modelagem de dados.

## Tecnologias Utilizadas
- **Power BI**: Visualização e modelagem de dados.
- **Azure MySQL**: Hospedagem da base de dados.
- **DAX**: Análises e cálculos avançados.
- **Linguagem M (Power Query)**: Transformação e limpeza de dados.

---

## Etapas do Projeto

### 1. Criação da Instância no Azure MySQL
- Configuramos uma instância MySQL no Azure com as configurações recomendadas.
- Importamos o banco de dados disponível no GitHub para a instância.

### 2. Integração com Power BI
- Conectamos o Power BI ao banco MySQL no Azure usando as credenciais de acesso.

### 3. Transformações de Dados
Realizamos as seguintes transformações na base de dados:
- **Cabeçalhos e Tipos de Dados:** Ajustamos os nomes dos campos e garantimos que cada coluna tivesse o tipo de dado correto (ex.: valores monetários foram convertidos para `Decimal Number`).
- **Tratamento de Valores Nulos:**
  - Identificamos colaboradores sem gerentes (nulos em `Super_ssn`) e validamos as informações.
- **Mesclas e Agrupamento de Tabelas:**
  - **Colaboradores e Departamentos:** Mesclamos as tabelas para adicionar os nomes dos departamentos aos colaboradores, utilizando uma junção do tipo `Inner`.
  - **Colaboradores e Projetos:** Associamos os colaboradores aos seus respectivos projetos para facilitar as análises. Criamos uma nova tabela agrupada e juntamos com a tabela de projetos.
- **Colunas Complexas:**
  - Criamos combinações únicas de `Nome do Departamento` e `Localização` para auxiliar na modelagem futura.

### 4. Visualizações Criadas
No Power BI, criamos visuais como:
- Gráficos de barras e linhas para análise de salários por projeto.
- Tabelas dinâmicas com detalhes de colaboradores, gerentes, salários e horas trabalhadas.
- Indicadores (KPIs) para monitorar métricas como idade mínima e máxima, média por departamento e média de idade por horas totais.

---

## Resultado Final
- Geramos um modelo confiável e limpo no Power BI.
- O relatório permite análises dinâmicas sobre colaboradores, projetos e departamentos, com insights úteis para decisões estratégicas.


---

### Autor
Rodrigo

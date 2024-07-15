# Criando-um-Dashboard-corporativo-com-integra-o-com-MySQL-e-Azure

Criando um Dashboard corporativo com integração com MySQL e Azure. A transformação dos dados resultou em um conjunto pronto para análise.
Foi estabelecida a conexão entre o MySQL e o Power BI, e realizada a limpeza e aplicação de filtros.
Configurando o Azure - criando uma instância MySQL na Azure Usando o arquivo “script_bd_company.sql”, estruturando o banco com tabelas e preenchimento com dados iniciais. 
Estabelecida uma conexão direta entre o Power BI Desktop e o MySQL na Azure.
Após importado foram feitas as correções na base com ajuste de erros no cabeçalho, tratamento de nulos que foram mantidos, conversão dos valores monetários para decimal fixo. 
Eliminando colunas que não ajudavam na analise, visando a melhoria de desempenho no relatório e analises mais limpas.
Mescla das colunas “employee” e “departament” via Power query, resultando na tabela “Departamento_Empregado”, usando como base “Ssn” de “employee” e “Mgr_ssn” de “departament” para assim conseguir indicar o departamento do empregado.
Realizada a associação entre colaboradores e gerentes, empregando uma consulta SQL na Azure que ligava cada funcionário ao seu supervisor. A consulta gerou uma tabela com as colunas "EmployeeName" e "ManagerName".
Logo se nome do funcionário fosse "John B Smith", "Franklin T Wong" ou "Ahmad V Jabbar", ele seria classificado como "Gerente", caso contrário seria classificado como "Colaborador", além disso foi mesclado as tabelas "company departament" e "company dept_locations" em uma única tabela "Department By Local".

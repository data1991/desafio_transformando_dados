# <img src="https://avatars1.githubusercontent.com/u/26231823?s=280&v=4" width="80" height="80"> Processando e Transformando Dados com Power BI
Desafio de Projeto - Processando e Transformando Dados com Power BI

# Objetivo do Projeto:
Processar os Dados de um arquivo .csv fornecido, transformá-los com Power BI e criar um relatório empresarial para saber se não houve problemas com os dados.

# Ferramentas Utilizadas 

#### . Azure . Power BI 

# Passo a Passo e Dicas Úteis

### Etapas de Processamento:

1. Criei uma instância na Azure par MySQL - Dica: use uma conta organizacional do tipo (IE- Instituição de Ensino), para evitar conflitos.
2. Criei o banco de dados com a base fornecida.
3. Integrei o Power BI com MySQL Azure - Dicas: instale o Visual Studio 2019 ou se já tiver instalado vá em Windows Updade e verifique se há alguma atualização de versão Windows e componentes do Visual Studio 2019, baixe a versão do Conector 8.0.28 ou 8.0.32, pois são as versões mais compatíveis com Windows 10 e Power BI por último verifique se você inseriu as credenciais do Azure no Power BI corretamente para evitar erros desnecessários.
4. Verifique a base de dados fornecida.

   ### Etapas de Transformação:

   1. Fiz o Renome dos cabeçalhos de todas as colunas das tabelas - Dica: você pode fazer isso clicando duas vezes no cabeçalho da coluna.
   2. Modifiquei os valores de "Salary" da tabela azure_company employee para o tipo (Número decimal fixo).
   3. Modifiquei os valores de "Hours" da tabela azure_company works_on para o tipo (Numeral inteiro).
   4. Na coluna "Hours" havia uma inconsistencia de dados 0 que transformei - Dica: para fazer isso selecione a coluna "Hours" com um clique e vá para a guia Página Inicial, nas opções da guia, clique em Substituir Valores, insira em Valor a Ser Localizado 0 e em Substituir por um valor de sua preferência.
   5. Separar colunas complexas só se for o caso, por exemplo, um endereço completo que tenha vários complementos.
   6. Para mesclar consultas "employee" e "departament" para criar uma tabela "employee" com o nome dos departamentos associados aos colaboradores -Dica: não precisa criar uma nova tabela "employee", uma vez que ela já existe. Na própria tabela azure_company employee, adicionei uma coluna chamada "Departament name". Para fazer isso vá até a tabela "employee", na guia Adicionar Coluna, clique na opção Coluna de Exemplos, vai aparecer uma coluna em branco renomeie como "Departament name".
   7. Repita o passo anterior para criar as colunas de "collaborators" que é a coluna que você vai incluir os valores de cada "Last Name" e "First Name", coluna de "Managers" e uma coluna chamada "Departament location", com os nomes dos respectivos departamentos e localizações. Não esqueçam de atualizar depois que fizerem cada modificação.
   8. O penúltimo passo do documento eu desconcideraria, mas como pode ser relevante é melhor fazer - Dica: duplique a tabela de "employee" e faça um Renome para azure_company collaborators_managers na guia Página Inicial, clique na opção Agrupar por, na tela que irá aparecer deixe o tipo de agrupamento como Básico escolha a coluna que você quer agrupar dê um nome para ela, em Operação escolha Max e em Coluna, escolha a coluna que você quer agrupar e em seguida aperte em "Ok".
   9. Segue os prints do projeto para vocês terem uma noção:

   ![print01](https://github.com/data1991/desafio_transformando_dados/assets/144493849/6ccf52a3-4615-418c-b041-520b1c7f2d71)
   ![Print02](https://github.com/data1991/desafio_transformando_dados/assets/144493849/1436d61c-2685-499c-85c1-a8a20e4886b5)
   ![print03](https://github.com/data1991/desafio_transformando_dados/assets/144493849/79b8addb-4913-4b4b-9289-0805eb9a753e)

  #### Página01 Relatório

  ![Página01](https://github.com/data1991/desafio_transformando_dados/assets/144493849/14a00bdc-9500-480d-b7e2-5aee1c3a7e84)

  #### Página02 Relatório

  ![Página02](https://github.com/data1991/desafio_transformando_dados/assets/144493849/03ff4292-2551-4833-a3e0-dfc2ca8df5a7)

  

  
   
   
   

   
       


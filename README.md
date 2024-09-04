Dashboard_de-Vendas_no_Power_BI
Projeto faz parte do curso de Engenharia de Dados proposto pela NTT DATA e Digital Innovation One.

Branches: master

DESCRIÇÃO Vamos para o primeiro desafio com Power BI? Neste projeto foi replicado duas páginas já criadas durante o curso com a sample disponibilizada.

Curso: Engenharia de Dados com Python NTT DATA e Digital Innovation One


Itens:

1: Importar a base de dados**

No nosso caso, a base de dados está em formato de excel, então, basta clicar no ícone "Pasta de trabalho do Excel", localizado no menu da "Página Inicial", e encontrar o arquivo de interesse para importar.


2: Visualizar a base de dados**

Após clicar para importar, teremos a janela de pré-visualização dos dados em que temos de selecionar a caixa com o nome da planilha do Excel. Ao clicar em "Transformar Dados", uma nova janela será aberta. Esta nova janela é o ambiente do Power Query, que é o editor de consultas do Power BI.


3: Tratamento de dados com o Power Query**

Nesse ambiente nós vamos fazer os tratamentos necessários na base de dados para que ela fique correta para utilizarmos no Power BI. Podemos começar alterando o nome da planilha, para algo mais intuitivo, como "Base de vendas", localizado na lateral esquerda, no ambiente "Config Consulta". Não é algo obrigatório, mas é uma boa prática.

A - Remover colunas desnecessárias**

Muitas vezes o Power BI acaba importando colunas em branco, por isso é bom clicar na opção "Transformar Dados", pode haver esses ou outros problemas. Como não há nenhuma informação na coluna, o melhor a se fazer é deletar essa coluna para não atrapalhar as nossas análises.

Para deletar uma coluna você pode selecioná-la e pressionar a
tecla Delete, ou pode selecioná-la e ir até a opção "Remover
Colunas", localizado no menu da "Página Inicial".

B - Remover Linhas em branco**

Também é comum que a base de dados tenha linhas em branco, para excluí-las, selecionamos a opção "Remover Linhas" > "Remover Linhas em Branco", na guia "Página Inicial".

C - Alteração na representação do nome do cliente**

As informações de nome estão no formato "Sobrenome, Nome". No entanto é interessante deixar essas informações no padrão "Nome Sobrenome".

Para fazer essa alteração de forma rápida e eficiente nós vamos selecionar a coluna "Nome Cliente" e utilizar a ferramenta "Coluna de Exemplos" > "da Seleção", localizada na guia "Adicionar Coluna". 

Ao escrever alguns exemplos, o programa entende o padrão e preencha as outras informações. Feito isso, basta clicar em Ok para que o Power Query crie uma coluna com essas informações. Com isso, pode-se renomear a coluna que foi adicionada e excluir a anterior, pois as duas tem as mesmas informações.

D - Alteração na representação da localidade**

A coluna de Localidade possui tanto o país quando o continente em uma mesma coluna, mas é interessante que sejam separadas, para uma melhor análise.

Para fazer essa separação vamos selecionar a coluna e usar a ferramenta "Dividir Coluna" > "Por Delimitador", localizada na guia "Transformar". Na aba que abrir, indicamos que o delimitador é o traço com espaços antes e depois, ou seja, " - ". Após isso, aparecerão duas colunas que podem ser renomeadas para "País" e "Continente".

E - Faturamento**

Podemos calcular a coluna de "Faturamento", que vai ser a
multiplicação da coluna "Preço Unitário" com a
coluna "Quantidade Vendida". Para fazer isso, vamos selecionar as uma das colunas e selecionar a opção "Padrão" > "Multiplicar", na guia "Adicionar Coluna". Na aba que abrir, selecione a coluna que deve multiplicar e depois renomeie a coluna.

F - Fechar e Aplicar**

Agora que finalizamos podemos clicar em "Fechar e Aplicar", na guia "Página Inicial", para voltar ao ambiente do Power BI com a base de dados tratada.


4: Criando o Dashboard**

Voltando para o Power BI, pois agora podemos trabalhar no ambiente "Relatório", onde criamos os gráficos e o Dashboard baseados nos dados importados. 

Começamos observando os dados e identificamos quais informações são importantes para por no Dashboard, como por exemplo, o valores totais de Faturamento, de custo e lucro, a quantidade de itens vendidos, e o faturamento por ano, mês, marca, produto e continente. Com essas informações, podemos construir o Dashboard abaixo.

<div  align="center"> 
  <img src="Imagens/Dashboard de Vendas - Sem a imagem de fundo.png">
</div>


5: Criando a tela de fundo do Dashboard**

Usamos o [Canva](https://www.canva.com/design/DAFX0ukBc2A/jL29j0Qb_z62u_MPSdnkAA/view?utm_content=DAFX0ukBc2A&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton) para fazer a construção da imagem de fundo representada abaixo, mas poderia ter usado o Microsoft PowerPoint.

<div  align="center"> 
  <img src="Imagens/Imagem de Fundo.png">
</div>


Observações:

O Dashboard construído ficou da seguinte maneira:

<div  align="center"> 
  <img src="Imagens/Dashboard de Vendas - Finalizado.png">
</div>


Podemos fazer seleções para representar aquilo que estamos interessados. Por exemplo, se selecionarmos o ano de 2018, a marca "Contoso" e o produto "Telephoto Conversion Lens X400", vemos a imagem abaixo.

<div  align="center"> 
  <img src="Imagens/Dashboard de Vendas - Finalizado com seleção.png">
</div>


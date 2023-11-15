# Projeto de conclusão de Disciplina: Aprendizado de Máquina
Este repositório é destinado a guardar os arquivos utilizados e desenvolvidos no projeto de consclusão da disciplina "Aprendizado de Máquina" do segundo semestre do Bacharel em Ciência e Tecnologia da Ilum - Escola de Ciência do Centro Nacional de Pesquisa em Energia e Materiais. O projeto foi desenvolvido com a integração das seguintes duplas formadas no inicio do semestre: "Aliança BA-AL", composta pelos estudantes "Mayllon Emmanoel Pequeno Santos Silva" e "Samuel Soares de Araújo", e pela dupla "Nemphis & Nempharey", composta pelos estudantes "Davi José de Araújo Pereira" e "Diogo Pereira de Lima Carvalho", consistindo numa análise de um conjunto de dados de importantes propriedades de materiais Supercondutores tendo como alvo a predição de sua temperatura crítica.

Em um primeiro momento foi formulado um notebook de preparação dos dados com base nos exercícios de análise exploratória do conjunto de dados escolhido. Para isso, utilizamos ferramentas visuais: gráficos de correlação, histogramas, espalhamento, tudo isso para uma melhor visualização da distribuição dos dados, além de uma explicação mais detalhada sobre os atributos e sua relevância cientifica. Por se tratar de um conjunto de dados consideravelmente grande, optamos por realizar a seleção de atributos pelo método VIF, que nos retornou 29 atributos mais relevantes. Com isso reduzimos o número de atributos do nosso conjunto de dados de 82 atributos para 29. Tendo feito a seleção, criamos um novo dataset atualizado e salvamos em um arquivo csv "Superconductors_dataset_2" com as features reduzidas, será esse arquivo que utlizaremos nos notebook com os modelos. Abaixo temos uma descrição do que contém em cada notebook e seu respectivo autor no projeto.

Notebook 1 (Notebook_1_Preparacao_Dados.ipynb): Contém a análise dos atributos, plots de esplhamento, calor e histogramas, seleção da features pelo método VIF, criação do novo conjunto de daos com atributos reduzidos
Autores: Davi J.A. Pereira, Diogo P. de L. Carvalho, Mayllon E.P.S. Silva, Samuel S. de Araújo

Notebook 2 (xxxxxxx.ipnyb): 
Autor: Diogo P. de L. Carvalho

Notebook 3 (xxxxxxx.ipnyb): 
Autor: Samuel S. de Araújo

Notebook 4 (Notebook_4_RANSAC_knn_RG.ipynb): Contém a análise de um modelo robusto (RANSAC) com suas versões de dimensionalidade reduzida pelo StandardScaler e por transformação linear com PCA em comparação com modelos de Regressão Linear e kNN.
Autor: Mayllon E.P.S. Silva

Notebook 5 (xxxxxxx.ipnyb):
Autor: Davi J.A. Pereira

Conclusão:

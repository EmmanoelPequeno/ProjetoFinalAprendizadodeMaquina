# Projeto de conclusão de Disciplina: Aprendizado de Máquina

*Os que se encantam com a prática sem a ciência são como os timoneiros que entram no navio sem timão nem bússola, nunca tendo certeza do seu destino”. - Leonardo da Vinci*

Este repositório é destinado a guardar os arquivos utilizados e desenvolvidos no projeto de consclusão da disciplina "Aprendizado de Máquina" do segundo semestre do Bacharel em Ciência e Tecnologia da Ilum - Escola de Ciência do Centro Nacional de Pesquisa em Energia e Materiais. O projeto foi desenvolvido com a integração das seguintes duplas formadas no inicio do semestre: "Aliança BA-AL", composta pelos estudantes "Mayllon Emmanoel Pequeno Santos Silva" e "Samuel Soares de Araújo", e pela dupla "Nemphis & Nempharey", composta pelos estudantes "Davi José de Araújo Pereira" e "Diogo Pereira de Lima Carvalho", consistindo numa análise de um conjunto de dados de importantes propriedades de materiais Supercondutores tendo como alvo a predição de sua temperatura crítica.

Em um primeiro momento foi formulado um notebook de preparação dos dados com base nos exercícios de análise exploratória do conjunto de dados escolhido. Para isso, utilizamos ferramentas visuais: gráficos de correlação, histogramas, espalhamento, tudo isso para uma melhor visualização da distribuição dos dados, além de uma explicação mais detalhada sobre os atributos e sua relevância cientifica. Por se tratar de um conjunto de dados consideravelmente grande, optamos por realizar a seleção de atributos pelo método VIF, que nos retornou 29 atributos mais relevantes. Com isso reduzimos o número de atributos do nosso conjunto de dados de 82 atributos para 29. Tendo feito a seleção, criamos um novo dataset atualizado e salvamos em um arquivo csv "Superconductors_dataset_2" com as features reduzidas, será esse arquivo que utlizaremos nos notebook com os modelos. Abaixo temos uma descrição do que contém em cada notebook e seu respectivo autor no projeto.

Modelos abordados durante o projeto: RANSACRegressor, Regressão Linear, k-NN, Baseline, Árvore de decisão, floresta aleatória, HuberRegressor, Theil-SenRegressor, RidgeRegressor

Notebook 1 (Notebook_1_Preparacao_Dados.ipynb): Contém a análise dos atributos, plots de esplhamento, calor e histogramas, seleção da features pelo método VIF, criação do novo conjunto de daos com atributos reduzidos |
Autores: Davi J.A. Pereira, Diogo P. de L. Carvalho, Mayllon E.P.S. Silva, Samuel S. de Araújo

Notebook 2 (xxxxxxx.ipnyb): descrição |
Autor: Diogo P. de L. Carvalho

Notebook 3 (xxxxxxx.ipnyb): descrição |
Autor: Samuel S. de Araújo

Notebook 4 (Notebook_4_RANSAC_knn_RG.ipynb): Contém a análise de um modelo robusto (RANSAC) com suas versões normalização padrão pelo StandardScaler e por redução de dimensionalidade com PCA em comparação com modelos de Regressão Linear e kNN. |
Autor: Mayllon E.P.S. Silva

Notebook 5 (Notebook_5_Huber_TheilSen.ipnyb): Contém tambpem a análise e explicação do funcionamento de dois modelos robustos (Huber Regressor e Theil-Sen Regressor) e algumas comparações com o modelo de Regressão Linear. |
Autor: Davi J.A. Pereira

Algumas orientações ao leitor:
<ul>
  <li>O notebook de preparação de dados é relativamente extenso e o processo de seleção de aributos pelo método VIF demorado. Com isso, o resultado desse processo está no arquivo CSV "Superconductors_dataset_2", não necessitando uma nova execução pelo usuário </li>
  <li>O arquivo "009-Dataset.csv" é um arquivo ditádito que só será utilizado nos notebooks em que serão trabalhados modelos robustos (RANSAC, Huber Regressor e Theil-Sen Regressor), não necessitando sua utilização nos demais notebooks </li>
  <li> O leitor não necessariamente precisa seguir a ordem dos notebooks, porém, é altamente recomendado que acesse "Notebook_4_RANSAC_knn_RG.ipynb" antes do "Notebook_5_Huber_TheilSen.ipnyb"</li>
  <li> As imagens "Tabela_var_deriva" e "Tabela_var_principais" serão apenas utilizadas no notebook de preparação dos dados e análise exploratória.</li>
  <li> As imagens "Brasao_BA-AL" e "Brasao_irmaos_magos" não é utilizada em nenhum dos notebook e serve apenas como recordação dos brasões que utilizamos em nosso notebooks durante o decorrer da disciplina</li>
</ul>

Conclusão:
A partir das comparações entre os diversos modelos que testamos em nosso conjunto de dados podemos afirmar de modo geral que os modelos de "kNNRegressor" e "Árvore de decisão" obtiveram melhores resultados na previsão de valores de temperatura crítica com base nos atributos de nosso dataset se comparados a outros modelos. Cada notebook terá suas conclusões mais detalhadas sobre os resultados do uso de cada modelo.

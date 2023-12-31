# Projeto de conclusão de Disciplina: Aprendizado de Máquina

*"Desde o nascer do sol no nordeste do país até se pôr em terras paulistas, nenhum bug de código sucederá a nossa presença. Todo erro de sintaxe há de penar quando o poder da Dualidade Mago-Cavaleiro enfrentar!" - (Adaptado do juramento da Aliança BA-AL, por sua vez adaptado do juramento da tropa dos lanternas verde)*

Este repositório é destinado a guardar os arquivos utilizados e desenvolvidos no projeto de consclusão da disciplina "Aprendizado de Máquina" do segundo semestre do Bacharel em Ciência e Tecnologia da Ilum - Escola de Ciência do Centro Nacional de Pesquisa em Energia e Materiais (CNPEM). O projeto foi desenvolvido com a integração das seguintes duplas formadas no inicio do semestre: "Aliança BA-AL", composta pelos estudantes "Mayllon Emmanoel Pequeno Santos Silva" e "Samuel Soares de Araújo", e pela dupla "Nemphis & Nempharey", composta pelos estudantes "Davi José de Araújo Pereira" e "Diogo Pereira de Lima Carvalho", que juntas formam a "Dualidade Mago-Caveleiro". O projeto consiste numa análise de um conjunto de dados de importantes propriedades de materiais Supercondutores e o teste de diversos modelos lineares tendo como alvo a predição de sua temperatura crítica.

Supercondutores são materiais que, quando resfriados abaixo de uma temperatura crítica específica, exibem uma propriedade notável chamada supercondutividade. A supercondutividade é um fenômeno fascinante com aplicações práticas e implicações significativas para a tecnologia e a pesquisa científica. Apesar dos desafios técnicos, os supercondutores continuam a ser uma área de intensa pesquisa e desenvolvimento. Em nosso dataset, atributos como "Massa atômica", "Raio Atômico", "Calor de fusão", dentre outros, serão impotantes para a previsão dos valores da temperatura crítica do supercondutor.

Em um primeiro momento foi formulado um notebook de preparação dos dados com base nos exercícios de análise exploratória do conjunto de dados escolhido. Para isso, utilizamos ferramentas visuais: gráficos de correlação, histogramas, espalhamento, tudo isso para uma melhor visualização da distribuição dos dados, além de uma explicação mais detalhada sobre os atributos e sua relevância cientifica. Por se tratar de um conjunto de dados consideravelmente grande ("train.csv"), optamos por realizar a seleção de atributos pelo método VIF, que nos retornou 29 atributos mais relevantes. Com isso reduzimos o número de atributos do nosso conjunto de dados de 82 atributos para 29. Tendo feito a seleção, criamos um novo dataset atualizado e salvamos em um arquivo csv "Dataset_superconductors_2" com as features reduzidas, será esse arquivo que utlizaremos nos notebook com os modelos. A partir disso, elaborou-se outros 4 notebooks com a aplicação de modelos de aprendizado de máquina com esse dataset, sendo que cada notebook foi realizado por um integrando diferente do projeto. Os modelos contemplados nesses cadernos foram: RANSACRegressor, Regressão Linear, k-NN, Baseline, Árvore de decisão, floresta aleatória, HuberRegressor, TheilSenRegressor e RidgeRegressor.

Abaixo temos uma descrição do que contém em cada notebook e seu respectivo autor no projeto.

Notebook 1 (Notebook_1_Preparacao_Dados.ipynb): Contém a análise dos atributos, plots de esplhamento, calor e histogramas, seleção da features pelo método VIF, criação do novo conjunto de dados com atributos reduzidos |
Autores: Davi J.A. Pereira, Diogo P. de L. Carvalho, Mayllon E.P.S. Silva, Samuel S. de Araújo

Notebook 2 (Notebook_2_Baseline_Decision-Rree_Random-Forest.ipnyb): Contém a análise e explicação do modelo <i>baseline</i>, além também dos modelos de árvore de decisão e floresta aleatória a partir da otimização de hiperparâmetros pelo <code>optuna</code>.
Autor: Diogo P. de L. Carvalho

Notebook 3 (Notebook_3_RIDGE.ipynb): Contém a análise do modelo RIDGE com otimização usando o optuna.
Autor: Samuel S. de Araújo

Notebook 4 (Notebook_4_RANSAC_knn_RG.ipynb): Contém a análise de um modelo robusto (RANSAC) com suas versões normalização padrão pelo StandardScaler e por redução de dimensionalidade com PCA em comparação com modelos de Regressão Linear e k-NN. |
Autor: Mayllon E.P.S. Silva

Notebook 5 (Notebook_5_Huber_TheilSen.ipnyb): Contém também a análise e explicação do funcionamento de dois modelos robustos (Huber Regressor e Theil-Sen Regressor) e algumas comparações com o modelo de Regressão Linear e k-NN. |
Autor: Davi J.A. Pereira

Em relação à organização dos arquivos desse projeto, há duas pastas que reunem os notebooks citados e os arquivos associados a esses, além de duas imagens de cunho simbólicas "Brasao_BA_AL.png" e "Brasao_irmaos_magos.png" que são os brasões que representam as duplas envolvidas no projeto. Na pasta "Notebook_de_Preparacao_de_dados", há o Notebook 1 em que se realizou a análise exploratória e a seleção de atributos do dataset, duas imagens utilizadas neste notebook acerca do dataset utilizado e o próprio dataset em formato de valores separados por vírgulas (CSV) em sua forma publicada, sem as modificações realizadas durante este projeto. Já na pasta "Notebooks_modelos_utilizados", há os Notebooks 2, 3, 4 e 5 da aplicação de modelos de aprendizado de máquina com o dataset, além de dois arquivos em formato de valores separados por vírgulas (CSV), sendo o dataset após a seleção de atributos realizada pelo Notebook 1 e um dataset utilizado como exemplificação em um dos notebooks. 

Algumas orientações ao leitor:
<ul>
  <li>O notebook de preparação de dados é relativamente extenso e o processo de seleção de aributos pelo método VIF demorado. Com isso, o resultado desse processo está no arquivo CSV "Superconductors_dataset_2", não necessitando uma nova execução pelo usuário </li>
  <li>O arquivo "Dataset_exemplo_robusto.csv" é um arquivo ditádito que só será utilizado nos notebooks em que serão trabalhados modelos robustos (RANSAC, Huber Regressor e Theil-Sen Regressor), não necessitando sua utilização nos demais notebooks </li>
  <li> O leitor não necessariamente precisa seguir a ordem dos notebooks, porém, é altamente recomendado que acesse "Notebook_4_RANSAC_knn_RG.ipynb" antes do "Notebook_5_Huber_TheilSen.ipnyb"</li>
  <li> As imagens "Tabela_var_deriva" e "Tabela_var_principais" serão apenas utilizadas no notebook de preparação dos dados e análise exploratória.</li>
  <li> As imagens "Brasao_BA-AL" e "Brasao_irmaos_magos" não é utilizada em nenhum dos notebook e serve apenas como recordação dos brasões que utilizamos em nosso notebooks durante o decorrer da disciplina</li>
</ul>

Conclusão:
A partir das comparações entre os diversos modelos que testamos em nosso conjunto de dados podemos afirmar de modo geral que os modelos de "kNNRegressor" e "Árvore de decisão" obtiveram melhores resultados na previsão de valores de temperatura crítica com base nos atributos de nosso dataset se comparados a outros modelos. Para além do kNN e Árvore de decisão, os modelos demais modelos lineares explorados e tratados também obtiveram significativo papel em nosso projeto. Cada notebook terá suas conclusões mais detalhadas sobre os resultados do uso de cada modelo.


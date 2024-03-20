# Análise de Crédito com Inteligência Artificial
Este projeto em Python foi desenvolvido na IDE Jupyter para facilitar a visualização das informações em forma de gráfico. O intuito é analisar uma base de dados de clientes e definir o score de crédito de acordo com informações do mesmo criar uma Inteligência Artificial que consiga definir se o score de crédito é ruim, ok ou bom.

### Funcionamento
- Com o pandas, importar a base de dados em csv para uma variável;
- Exibir a base de dados e suas informações para facilitar a analise e melhor visualização;  
- Analisar e identificar colunas que estejam em formato object e usar o LabelEncoder do sklearn para codificar as colunas para números, para assim ser possível que a IA consiga ler as informações;
- Após codificar as colunas para números iremos dividir a tabela em 2 variáveis:
     → y: Será a coluna da base de dados na qual a IA irá prever;
     → x: Será o resto da base de dados, sem a coluna que a IA irá prever;
- Com a função train_test_split da biblioteca sklearn iremos separar 70% das informações para treino e 30% para o teste da IA;
- Importar as IA’s RandomForestClassifier e KNeighborsClassifier e treina-las com a função .fit()
- Fazer a previsão individual de cada com .predict()
- Imprimir a precisão de cada uma com a função accuracy_score()
- A Inteligência Artificial que tiver a melhor precisão no treino será usada para fazer o teste com novas informações (para garantir que ela não apenas decorou);
- Ao final ainda é possível exibir o peso de cada coluna para dedução das informações;

### Adaptações
As adaptações necessárias para o correto funcionamento do código na sua máquina será apenas editar a base de dados, as colunas que necessitam de codificação e a coluna a ser prevista pela IA.<br>
Caso for de sua preferência é possível mudar a porcentagem de dados utilizados para treino/teste.

### Tecnologias Usadas
- pandas
- sklearn
     → LabelEncoder
     → train_test_split
     → RandomForestClassifier
     → KNeighborClassifier
     → accuracy_score




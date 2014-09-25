T2 ORI UFSCAR 2014
==================
Tabelas hash
------------
###Introdução
-----------
Tabelas hash são estruturas de dados voltadas para a rápida recuperação de dados. Seu principal custo não está no cálculo da função, mas na resolução das possíveis colisões. Esse custo está na quantidade média de sondagens realizadas até localizar um dado item ou falhar na busca.

Avaliar esse desempenho de maneira prática é uma forma interessante de visualizar o potencial dessas tabelas.

O trabalho deve ser desenvolvido em grupos de 3 ou 4 alunos. A penalidade por não seguir essa especificação é de 1 ponto por aluno a mais ou a menos.

###O que fazer
------------
Deve ser implementada uma tabela hash com as operações de inserção e busca. O tratamento de colisões adotado deve ser a sondagem linear (linear probing). Os dados a serem inseridos são números inteiros positivos e não deve haver repetições de chaves.

Os testes devem ser realizados com tabelas de tamanhos variados, mas obrigatoriamente o tamanho máximo da tabela deve ser um número primo. A quantidade de tamanhos de tabelas diferentes vai depender de como a discussão no relatório será conduzida.

A tabela deve ser testada nas seguintes condições:
> * Com ocupação de 60%
* Com ocupação de 75%
* Com ocupação de 90%

Cada teste deve ser feito da seguinte forma:
> * Criar uma tabela vazia
* Inserir dados aleatórios até que a ocupação desejada seja atingida
* Levantar o número médio de sondagens bem sucedidas (descrição abaixo)
* Levantar o número médio de sondagens mal sucedidas (descrição abaixo)

Para o levantamento do número médio de sondagens bem sucedidas:
> * Gerar consultas com valores que existem na tabela (todos eles)
* Para cada consulta, contar o número de sondagens realizadas até que o item seja encontrado
* Calcular o número médio das sondagens (soma das sondagens dividida pelo número de consultas)

Para o levantamento do número médio de sondagens mal sucedidas:
> * Gerar consultas com valores que não existem na tabela, em número 5 vezes maior que a quantidade de elementos existentes
* Para cada consulta, contar o número de sondagens realizadas até detectar  a falha na pesquisa
* Calcular o número médio das sondagens (soma das sondagens dividida pelo número de consultas)

Deve ser gerado um relatório descrevendo os experimentos, de conteúdo básico:
> * Capa
* Introdução
* Objetivos
* Descrição dos experimentos
* Resultados obtidos (com tabelas e gráficos) com discussão
* Conclusões dos experimentos
* Bibliografia consultada

###O que entregar
-----------------
Deve ser entregue o relatório, no formato PDF. Outros formatos não serão aceitos. O texto deve ter, aproximadamente, 2cm de margens e ser escrito em fonte tamanho 12 (exceto pelos títulos das seções); sugere-se fonte Arial. As figuras, gráficos e tabeças devem ser numeradas e referenciadas exclusivamente pelo número no texto (exemplo ok: "...como mostra a Figura 3..."; exemplo errado: "...na tabela seguinte..."). Gráficos e figuras devem ser numerados com valores arábicos (1, 2, 3...) e tabelas, em romanos (I, II, III...). Todas as figuras, gráficos e tabelas devem ter uma legenda descritiva consistente; nas figuras e gráficos, a legenda deve ficar abaixo; nas tabelas, acima.

Também deve ser entregue o código fonte do programa usado para gerar os resultados.

Apenas um dos elementos do grupo deve submeter o trabalho no Moodle.

###Critérios de avaliação
-------------------------
Será avaliado somente o relatório, principalmente quanto a seu conteúdo, discussão e conclusões.

O código enviado não será avaliado e será consultado apenas para verificar a consistência com os resultados apresentados. O código não precisa, portanto, ser "bonito" nem produzir interface amigável, visto que somente os dados da simulação são relevantes.

###Observações
--------------
O plágio (ou qualquer ação ilícita) não será tolerado e será punido conforme expresso no plano de ensino.

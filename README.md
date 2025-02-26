# 🍷 Prevendo a qualidade de vinhos 🍷

## Introdução

A noção de qualidade é apenas mais uma das inúmeras referências criadas pelo gênero humano. Como o termo tem diversas utilizações, o seu significado nem sempre é de definição clara e objetiva. Ela se aplica a
incontáveis situações. Por exemplo, quando se fala da qualidade de vida das pessoas de um país ou região, da qualidade da água que se bebe, do ar que se respira, do serviço prestado por uma determinada empresa, etc. No que diz respeito aos produtos e/ou serviços vendidos no mercado, as definições para qualidade se referem a conformidade com as exigências dos clientes, relação custo/benefício, adequação ao uso, utilidade, etc. Enfim, o termo é geralmente empregado para significar "excelência" de um produto ou serviço¹.

No mundo do vinho, o conceito de qualidade encerra toda a complexidade que o caracteriza e, muitas vezes, confunde-se com a percepção dos consumidores, a qual varia de maneira quase infinita. Por esta razão, é absolutamente necessário fazer a diferença entre qualidade intrínseca e qualidade percebida. A primeira diz respeito aos atributos que o produto apresenta e a segunda diz respeito à capacidade que cada consumidor ou grupo de consumidores tem de percebe-lo. Sendo o vinho um líquido constituído de água, substâncias orgânicas e minerais, sua qualidade intrínseca repousa sobre os seguintes pilares: ausência de defeitos tecnológicos; concentração dos componentes orgânicos e minerais; harmonia dos teores dos referidos componentes e; expressão da tipicidade olfativa e gustativa¹.

A ausência de defeitos tecnológicos é a base de tudo: não há como um produto ter qualidade se apresentar um defeito, qualquer que seja. A concentração dos componentes orgânicos e minerais em um vinho deve ser rica e complexa, de modo que sua estrutura (corpo) impressione imediata e positivamente o degustador e evite passar uma impressão de aguado, magro e sem expressão. Também não pode ser excessiva, sob pena de torna-Io difícil de beber¹. 

Se a concentração em compostos orgânicos e minerais forma e estrutura (corpo) do vinho, então a mesma está na base da sua alta qualidade intrínseca. Mas é imperativo que haja harmonia dos teores dos elementos que
a compõem. E é por este fator que explica-se porque há poucos vinhos de qualidade realmente diferenciada: é que, quanto maior a concentração desses elementos, mais dificilmente os mesmos estarão em absoluta harmonia. Um exemplo típico é o de um tinto encorpado, que tende a ser excessivamente tânico¹.

Seguindo os preceitos de qualidade definidos por critérios físico-químicos dos vinhos produzidos na regição norte de Portugal, no ano de 2009. Foram avaliados vinhos de dois tipos (Tinto e Branco). Ao final da avaliação dos valores mensurados para cada variável, atribuiu-se uma escala de notas variando de 1 a 10 para a classificação da qualidade dos vinhos produzidos na região Norte de Portugal.


## Fonte de dados

Os dados foram obtidos por meio do portal da UC Irvine Machine Learning Repository², disponíveis em: https://archive.ics.uci.edu/dataset/186/wine+quality 

## Variáveis de qualidade analisadas 

### ⚗️ Acidez Fixa (fixed_acidity)

A acidez fixa de um vinho é a soma dos ácidos naturais presentes na bebida, como o tartárico, málico, cítrico, succínico e láctico. A acidez fixa é medida em gramas de ácido tartárico por litro. A acidez fixa é importante pois preserva as qualidades naturais do vinho, como a cor, influencia o perfil sensorial, o equilíbrio e a longevidade da bebida, enriquece a experiência gastronômica ao harmonizar com uma variedade de pratos. 

### ⚗️ Acidez Volátil (volatile_acidity)

A acidez volátil de um vinho é a presença de ácidos gasosos, como o ácido acético, que podem ser percebidos pelo olfato.  É formada por bactérias acéticas que oxidam o álcool em ácido acético, que é o principal composto responsável pelo aroma de vinagre. Este composto secundário que tem cheiro de removedor de esmalte ou diluente de tinta. A acidez volátil é regulamentada por lei. 

### ⚗️ Ácido cítrico (citric_acid)

O ácido cítrico é um ácido orgânico fraco que pode ser adicionado ao vinho para aumentar a acidez e dar um sabor fresco. É também usado como estabilizador para evitar névoas férricas. O ácido cítrico pode aumentar o crescimento de micróbios indesejados. Alguns tipos de bactérias podem transformar ácido cítrico em acético, o que pode ser um problema sério.

### ⚗️ Açúcar residual (residual_sugar)

O açúcar residual é o açúcar natural da uva que sobra após a fermentação do vinho. Ele é um subproduto natural do processo de fermentação e pode afetar a textura e o sabor do vinho. 

### ⚗️ Cloretos (chlorides)

O teor de cloretos pode afetar o sabor do vinho, podendo conferir um sabor salgado ao produto final.

### ⚗️ Dióxido de enxofre livre (free_sulfur_dioxide) Dióxido de enxofre total (total_sulfur_dioxide) 

O dióxido de enxofre (SO2) é uma substância química que é adicionada ao vinho para conservá-lo e protegê-lo da oxidação. É também conhecido como sulfito. 

### ⚗️ Densidade (density)

A densidade do vinho é uma medida que indica a quantidade de sólidos dissolvidos no líquido, como açúcares, ácidos e outros compostos. É uma característica que influencia o sabor e aroma do vinho, além de ser importante para avaliar a qualidade e o potencial de envelhecimento. 

### ⚗️ pH (pH) 

O pH do vinho varia entre 2,8 e 4,5, dependendo do tipo de vinho, da casta, do cultivo e da safra. Vinhos brancos, geralmente têm um pH entre 3,0 e 3,3. Vinhos brancos de alta qualidade têm um pH entre 3,1 e 3,4. Vinhos tintos, geralmente, têm um pH entre 3,3 e 3,5. Vinhos tintos de alta qualidade têm um pH entre 3,3 e 3,6.

### ⚗️ Outros compostos a base de enxofre (sulfates)

Eventuais compostos derivados de enxofre que estejam sob forma livre no vinho.

## Tipo de modelo utilizado para predição

A previsão do índice de qualidade foi feita utilizando regressão logística. 

## Insigthis 

Com base no modelo obtido e na análise dos dados pôde-se constatar que:

### 💡A maioria dos vinhos (tanto tinto, quanto branco) foi classificada com notas entre 5 e 6.

### 💡Não foi observada a ocorrência de vinhos com nota máxima (10). 

### 💡As maiores notas (9) foram atingidas exclusivamente por vinhos brancos.

### 💡Os vinhos com maiores notas (8-9) apresentaram: 
####   🍷 Acidez fixada: 4,0-13,0 g/L de ácido tartárico
####   🍷 Acidez volátil: 0,1-0,9 g/L de ácido acético
####   🍷 Ácido cítrico: 0,01-0,78 mg/L de ácido cítrico
####   🍷 Açúcar residual: 0,0-20,0 g/L 
####   🍷 Dióxido de enxofre livre: 0,0-120 mg/L
####   🍷 Dióxido de enxofre total: 0,0-250 mg/L
####   🍷 Densidade: 0,90-1,00 g/ml
####   🍷 pH: 2,8-3,8
####   🍷 Teor alcoólico: 8,0-14,0 g/ml

## Referências

¹ GUERRA, C. C. O que é vinho de qualidade? EMBRAPA. Disponível em: https://www.infoteca.cnptia.embrapa.br/infoteca/bitstream/doc/974985/1/bonvivantv14n155p42dez2013.pdf. Acessado em: 26/02/2025. 

² UC Irvine Machine Learning Repository. Disponível em: https://archive.ics.uci.edu, acessado em: 26/02/2025.


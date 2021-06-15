<b>[PT-BR]</b> <br />
<b>Coletânea de médias móveis para TradingView</b>

<b>Resumo</b>
Essa é uma coletânea de médias móveis desenvolvidas em PineScript para a plataforma de análise técnica do <b>TradingView</b>.

<b>Motivação</b>
Para usar os diferentes tipos de médias móveis (por exemplo: simples, exponencial, etc.), é necessário inserir cada indicador separadamente.
Isso pode ser trabalhoso, necessidando a inclusão ou remoção dos indicadores toda vez que se deseja realizar a mudança.
Basicamente, o que este script faz, é permitir o uso dinâmico dessas médias móveis. 
Ou seja, é possível escolher o tipo de média móvel conforme a necessidade, facilitando a comparação e a criação de setups.

<b>Médias Móveis</b>

<b>1. Média Móvel Simples</b>

Definição

Média Móvel (MA) é um indicador baseado em preço, atrasado (ou reativo) que exibe o preço médio de um título durante um período de tempo definido. 
Uma Média Móvel é uma boa maneira de avaliar o momento, confirmar as tendências e definir áreas de suporte e resistência. 
Essencialmente, as médias móveis suavizam o "ruído" ao tentar interpretar gráficos. 
O ruído é composto de flutuações de preço e volume. Como uma Média Móvel é um indicador de atraso e reage a eventos que já ocorreram, 
ela não é usada como indicador preditivo, mas como indicador interpretativo, usado para confirmações e análises. 
De fato, as médias móveis são a base de várias outras ferramentas conhecidas de análise técnica, como as bandas de Bollinger e o MACD. 
Existem alguns tipos diferentes de médias móveis que seguem a mesma premissa básica e adicionam uma variação. 
Os mais notáveis são a Média Móvel Simples (SMA), a Média Móvel Exponencial (EMA) e a Média Móvel Ponderada (WMA).

Média Móvel Simples é uma Média Móvel não ponderada. 
Isso significa que todos os dias no conjunto de dados têm igual importância e têm o mesmo peso. 
À medida que cada novo dia termina, o ponto de dados mais antigo é descartado e o mais novo é adicionado ao início.

<b>2. Média Móvel Exponencial</b>

Definition
The Exponential Moving Average (EMA) is a specific type of moving average that points towards the importance of the most recent data and information from the market. 
The Exponential Moving Average is just like it’s name says - it’s exponential, weighting the most recent prices more than the less recent prices. 
The EMA can be compared and contrasted with the simple moving average.

Limitations
Although using the Exponential Moving Average has a lot of advantages when analyzing market trends, 
it is also uncertain whether or not the use of most recent data points truly affects technical and market analysis. 
In addition, the EMA relies on historical data as its basis for operating and because news, events, 
and other information can change rapidly the indicator can misinterpret this information by weighting the current prices higher than when the event actually occurred. 

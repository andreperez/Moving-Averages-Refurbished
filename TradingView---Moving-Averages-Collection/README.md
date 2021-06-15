# ![logo](images/Pine.png "Pine")

## Coletânea de Médias Móveis para TradingView

## Resumo

Essa é uma coletânea de médias móveis desenvolvidas em PineScript para a plataforma de análise técnica do **TradingView**.

## Motivação

Para usar os diferentes tipos de médias móveis (por exemplo: simples, exponencial, etc.), é necessário inserir cada indicador separadamente.
Isso pode ser trabalhoso, necessidando a inclusão ou remoção dos indicadores toda vez que se deseja realizar a mudança.
Basicamente, o que este script faz, é permitir o uso dinâmico dessas médias móveis. 
Ou seja, é possível escolher o tipo de média móvel conforme a necessidade, facilitando a comparação e a criação de setups.

---

### Definições

### Média Móvel

A Média Móvel (MA) é um indicador baseado em preço, atrasado (ou reativo) que exibe o preço médio de um título durante um período de tempo definido.
Uma Média Móvel é uma boa maneira de avaliar o momento, confirmar as tendências e definir áreas de suporte e resistência.
Essencialmente, as médias móveis suavizam o "ruído" ao tentar interpretar gráficos.
O ruído é composto de flutuações de preço e volume. 
Como uma Média Móvel é um indicador de atraso e reage a eventos que já ocorreram,
ela não é usada como indicador preditivo, mas como indicador interpretativo, usado para confirmações e análises.
De fato, as médias móveis são a base de várias outras ferramentas conhecidas de análise técnica, como as bandas de Bollinger e o MACD.
Existem alguns tipos diferentes de médias móveis que seguem a mesma premissa básica e adicionam uma variação.
Os mais notáveis são a Média Móvel Simples (SMA), a Média Móvel Exponencial (EMA) e a Média Móvel Ponderada (WMA).

### Média Móvel Simples

A Média Móvel Simples é uma Média Móvel não ponderada.
Isso significa que todos os dias no conjunto de dados têm igual importância e têm o mesmo peso.
À medida que cada novo dia termina, o ponto de dados mais antigo é descartado e o mais novo é adicionado ao início.

### Média Móvel Exponencial

The Exponential Moving Average (EMA) is a specific type of moving average that points towards the importance of the most recent data and information from the market.
It’s exponential, weighting the most recent prices more than the less recent prices.

Although using the Exponential Moving Average has a lot of advantages when analyzing market trends,
it is also uncertain whether or not the use of most recent data points truly affects technical and market analysis.
In addition, the EMA relies on historical data as its basis for operating and because news, events,
and other information can change rapidly the indicator can misinterpret this information by weighting the current prices higher than when the event actually occurred.

### Double Exponential Moving Average

The Double Exponential Moving Average (EMA) is a technical indicator that uses two moving averages to help confirm uptrends when price moves above average, and confirm downtrends when the price moves below average. A trend change might be occurring when the price moves in a direction away from the average. In addition, moving averages can be used to signify support and/or resistance territories.

The Double EMA has a quicker response when compared with traditional EMAs and can be used in the same ways. Remember that if you are using Double EMAs that it reacts quicker and therefore you should be planning your strategies around this information - alterations may be in order.

Traditional moving averages are good to use to identify trends in markets, but they don’t give much data when prices are choppy or not smooth. When price crosses the moving average or Double EMA, it is difficult to determine results and decide on when a trade will be profitable.

For this reason, it is great to pair the Double EMA with other technical indicators, or other price and/or fundamental analysis tools. By pairing the Double EMA, investors and traders can better determine market trends while looking at the big picture, and not getting hung up on the limitations or focusing on one sole indicator.

To conclude our limitations section, one thing to note would be the significance of reducing lag. Reducing lag can be beneficial in some instances, such as if there is a reversal in actual price. It can help get a trader out quickly and before any major losses occur. However, reduced lag may also result in something called overtrading; when an indicator provides a trader with too many signals at once. An indicator that has less lag is also more susceptible to reacting to small shifts in price that would normally not have a large effect. So remember that lag can be good at times, but at others it can really get in the way. It is up to the trader to decide whether or not lag is something they want or need from their indicator.

### Triple Exponential Moving Average

The Triple Exponential Moving Average (EMA) indicator was created to make it easier for traders to determine strength or weakness without the traditional lag associated with regular moving averages (MAs). In order to accomplish this, the Triple EMA takes multiple EMAs of the original EMA and then subtracts lag from the result.

Although the Triple EMA is known by many traders as a great indicator for reducing lag, it still has its faults as is true for any other indicator. MAs, for example, are very useful for trending markets, when price direction is particularly strong. When trends are choppy and price direction is weak, MAs, and the Triple EMA as well, may generate false signals as price fluctuates and the direction is in flux.

The Triple Exponential Moving Average reduces lag, smooths price fluctuations, and is an alternative to other moving averages because of its different calculation. The Triple EMA is shown as a single line. Its calculation takes multiple EMAs of the original EMA and then subtracts lag from the result.

### Weighted Exponential Moving Average

A média ponderada é qualquer média que multiplica fatores para fornecer diferentes pesos para diferentes dados. Na análise técnica, a média móvel ponderada (WMA) representa, especificamente, o valor de pesos que diminuem aritimeticamente. Assim, em um dia x, a WMA do último dia tem peso x, do penúltimo dia tem peso x-1 e assim sucessivamente até o dia 0.

A média móvel ponderada é utilizada para "solucionar" o problema de igualdade de pesos. Este indicador é calculado através da soma de todos os preços de fechamento dividido por um certo período de tempo e os multiplicando pela soma dos valores (pesos) de cada dia. Por exemplo, para uma média poderada de cinco dias, o preço de fechamento de hoje será multiplicado por cinco, o de ontem por quarto e assim por diante até que o primeiro dia na escala do período seja alcançado. Esses valores são então somados e dividos pela soma dos multiplicadores.

### Smoothed Moving Average

The Smoothed Moving Average compares recent prices to historical ones and makes sure they are weighed and considered equally. The calculation of this indicator does not reference a specific or fixed period, rather uses all available data in the series for analysis. The Smoothed Moving Average differs from the Exponential Moving Average (EMA) because it’s generally used with a longer time period.

The Smoothed Moving Average compares recent prices to historical ones and ensures they are analyzed with equal weight. The indicator does not refer to a fixed period when calculating results, but rather it uses all data available and does not remove specific data points once they have passed a specific time threshold.

### Least Squares Moving Averag

Least Square Moving Average is also called Linear regression moving average.
Moving linear regression may look similar to a moving average, but differs in its calculation. Moving averages are calculated using an average of closing prices, like with simple moving averages (SMA). Alternatively, they can be calculated by assigning greater weights to more recent prices and proportionately lower weights to prices farther in the past and then averaging those together. (In this case, the most common form is the exponential moving average, or EMA.)

Moving linear regression takes a continuous series of linear regression line endpoints and joins them together.

Based on these different methodologies, moving linear regression tends to hug price a lot more closely than moving averages of the same periodicity.

### Hull Moving Average

The Hull Moving Average (HMA) is a directional trend indicator. It captures the current state of the market and uses recent price action to determine if conditions are bullish or bearish relative to historical data.

The Hull differs from more traditional trend indicators like the Exponential Moving Average (EMA) and the Simple Moving Average (SMA). It is designed to reduce the lag often associated with those MAs by providing a faster signal on a smoother visual plane.

The Hull Moving Average (HMA) is a quick and smooth moving average that is distinct in its own nature. The HMA attempts to remove lag in its entirety, while simultaneously improving upon smoothing.

### Arnaud Legoux Moving Average (ALMA)

The ALMA is a technical analysis tool that aims to give investors and traders a more reliable trading signal by reducing the noise that can interfere with traditional moving averages. It eliminates the small fluctuations in an asset price to make the trend clearer.

The ALMA reduces price lag and creates a smoother line than other moving averages. Rather than a straightforward moving average for a certain period, it applies a moving average twice – from left to right as well as right to left.

The ALMA is a relatively new technical indicator, as many of them were developed during the 1970s, but it has quickly become popular. Arnaud Legoux and Dimitrios Kouzis Loukas developed the average in 2009 as they sought to address the weaknesses of simple moving averages (SMAs) and exponential moving averages (EMAs). They were inspired by Gaussian filters, which remove detail and noise to create a smooth image.

Legoux and Kouzis Loukas aimed to provide a leading indicator, as SMAs, EMAs and Smoothed Moving Averages (SMMAs) are considered lagging indicators.

No technical indicators are 100% accurate as they can sometimes generate false signals. You should never rely on a single indicator and always use a range of them when making trading decisions. 
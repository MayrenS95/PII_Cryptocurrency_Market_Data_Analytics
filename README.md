
<img style= "text-align: center;" src='Imagenes/logo henry.PNG'>
      
<h1 style="text-align: center;"><strong>PROYECTO INDIVIDUAL Nº2</strong></h1>
           
<h2 style="text-align: center;">Cryptocurrency Market Data Analytics</h2>
    
<h3><strong>Conexión API CoinGecko - Generación Dataframe</strong></h3>

<p style="text-align: justify;">Para llevar a cabo el presente proyecto, se hace uso de la API  pública que posee
CoinGecko, cuyo  objetivo es democratizar el acceso a las criptomonedas y dotar a los usuarios de información procesable. Asimismo,
indaga en el mundo de las criptomonedas para poder ofrecer información valiosa a sus usuarios a través de informes, publicaciones y boletines informativos sobre las criptomonedas, entre otros recursos.
</p>

<p style="text-align: justify;">Cuya documentación podemos encontrar en el siguiente enlace: <a href="https://www.coingecko.com/en/api/documentation">Documentación</a></p>

<img style= "text-align: center;" src='Imagenes\image.png'>

<ul>
<li style="text-align: justify;"> Se hace necesario entonces importar las librerias tanto de la API, como aquellas que nos permitirán hacer los análisis necesarios de los datos.</li>

<li style="text-align: justify;">Se procede entonces, a instanciar la función exportada de la libreria de CoinGecko
 definir el periodo sobre el cuál se hará el análisis de los datos.</li>

<li style="text-align: justify;"> Se define entonces la forma en la que se van a extraer los datos, para este caso se hace uso de una función, la cuál cuenta con los siguientes parámetros:</li>
<ol>
<li><strong>id_moneda:</strong> nombre de la moneda en página CoinGecko.</li>
<li><strong>vs_moneda:</strong> tipo de moneda en la que se traerá el valor de la misma.</li>
<li><strong>desde_fecha:</strong> fecha inicial.</li>
<li><strong>hasta_fecha:</strong> fecha final.</li>
<li><strong>precision:</strong>cantidad de decimales a tomar en cuenta.</li>

</ol>
<li>Se seleccionan las monedas que se van a emplear para el presente proyecto,
tomando como referencia el ranking de la página de CoinGecko, y otros artículos como los publicados por plus500.com y bussines inside.
</li>
<li>Se genera el dataframe con las siguientes variables por criptomoneda: precio, market cap y volumen total de transacción en unidades monetarias.</li>
</ul>
    
<h3><strong>EDA (Exploratory Data Analysis)</strong></h3>

<p style="text-align: justify;">Se procede a hacer uso de las funciones y gráficas pertinentes para hacer el análisis de los datos y llegar a las conclusiones necesarias para la toma de decisiones. Se evidencia lo siguiente:
</p>

<ul>
<li>No se encuentran valores nulos, ni duplicados dentro de las columnas o variables extraidas para generar el dataframe</li>
<img style="text-align: center;" src="Imagenes/heatmap-nulos.PNG">
<h4 style="text-align: center;">fig.1 Heatmap - Valores nulos</h4>

<li>Se evidencia la correlación positiva entre las variables precio y mercado de capitalización, mientras que en cuanto al total de transacciones no se observa que estas se encuentren relacionadas.</li>
<img  style="text-align: center;" src="Imagenes/pairplot.png">
<h4 style="text-align: center;">fig.2 Pairplot - Ethereum</h4>

<li>Se procede a gráficar el comportamiento histórico de los precios de las monedas, mercado de capitalización, para evidenciar tendencias.</li>

<li>Se gráfican también los puntos máximos en cuanto a precios y volumen transaccional</li>
</ul>

<h3><strong>KPI'S</strong></h3>

<p style="text-align: justify;">Observamos que los indicadores o Kpi's, nos permiten monitorear el comportamiento de las variables que intervienen en el valor de las criptomonedas, permitiendonos asi identificar tendencias, para la toma de decisiones oportunas y a futuro.</p>

<p style="text-align: justify;">Para este proyecto se tuvieron en cuenta indicadores como lo son la variación porcentual relativa del precio de las monedas, el valor promedio del volumen ransaccional en unidades monetarias para observar su significancia o uso por pate del publico objetivo, tambien se observa el comportamiento a lo largo del tiempo del activo circulante, que nos permite hacer estimaciones acerca del precio.</p>

<ol>
<li>Variación Relativa Precio Año anterior vs Año posterior (%)</li>
<li>Valor promedio diario transaccional, Valor promedio mensual transaccional, Valor promedio anual transaccional</li>
<li>Variación activo circulante anual(%)</li>
<li>Variación activo circulante mensual(%) </li>

</ol>


<h3><strong>Conclusiones</strong></h3>

<ul>
<li>En conclusión podemos decir que los cambios que sufren las criptomonedas como bitcoin, ethereum, polkadot, cardano, binance, litecoin se encuentran estrechamente ligados, pues los mismos tienen un comportamiento similar historicamente.</li>
<li>Asimismo, se encuentran criptomonedas como solana y polkadot que presentan un comportamiento historico que difiere de las anterioemente mencionadas.</li>

<li>A pesar de las fluctuaciones presentadas históricamente, el valor de bitcoin y ethereum sigue siendo el más representativo en contraste con las otras monedas analizadas en el presente proyecto.</li>

<li>A diferencia de las criptomonedas bitcoin y ethereum, la distribución de los datos de monedas como solana, polkadot, dogecoin, y demás monedas tomads en cuenta para el análisis, presentan outliers lo que implica que se han presentado eventos que han influido en el comportamiento de las mismas, se hace necesario realizar una investigación mas exhaustiva para conocer las causas de estos cambios.</li>

<li>Se evidencia que existe una correlación positiva entre las variables precio y capitalización del mercado, lo que se corresponde con la formula para el cálculo de las mismas, por su parte para la variable de volumen transaccional, no existe evidencia en cuanto a correlación con alguna de las variables anteriormente mencionadas.</li>

<li>El comportamiento histórico de las criptomonedas, en el periodo analizado nos permite concluir que se tuvo un tiempo de cosecha en lo que fue el año 2021, pues aquí el total de las monedas analizadas presentaron el valor máximo de cotización del mercado, siendo lideradas por los gigantes como bitcoin y etrhereum.</li>

<li>Con relación a lo anterior se evidencia un máximo en cuanto a volumen de transacción también para lo que es el año 2021 y 2022, teniendo en cuenta que el precio y capitalización del mercado disminuyo siginificativamenten en este ultimo año, debido a incertidumbre economica y el temor de las personas por invertir en este tipo de activos tan volatiles.</li>

<li>Observamos que los indicadores o Kpi's, nos permiten monitorear el comportamiento de las variables que intervienen en el valor de las criptomonedas, permitiendonos asi identificar tendencias, para la toma de decisiones oportunas y a futuro.</li>

<li>Para este proyecto se tuvieron en cuenta indicadores como lo son la variación porcentual relativa del precio de las monedas, el valor promedio del volumen ransaccional en unidades monetarias para observar su significancia o uso por pate del publico objetivo, tambien se observa el comportamiento a lo largo del tiempo del activo circulante, que nos permite hacer estimaciones acerca del precio.</li>
</ul>

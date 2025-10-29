<!-- ===================== PORTADA ===================== -->

<div style="text-align:center; margin-bottom: 2rem;">

  <h1 style="margin-bottom: 0.2rem; font-weight:600; font-size:2rem;">
    Importancia de la Visualización de Datos
  </h1>

<div style="margin-top:1rem;">
    <img src="https://github.com/user-attachments/assets/a80d578b-0ff5-4241-8683-7ddba19c8806"
         alt="UPS Logo"
         width="220"/>
</div>
  <div style="font-size:0.95rem; line-height:1.4;">
    <em>Carrera:</em> Ingeniería en Ciencias de la Computación<br/>
    <em>Periodo:</em> 67<br/>
    <em>Estudiante:</em> Erick Zhigüe Granda
  </div>

</div>

<hr/>

<!-- ===================== INTRODUCCIÓN ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">1. Introducción: ¿Por qué es importante visualizar datos?</h2>

<p style="text-align:justify;">
La visualización de datos es una etapa crítica del análisis estadístico y científico. 
No se trata solo de “hacer gráficos bonitos”, sino de <strong>ver patrones, tendencias, anomalías y relaciones</strong> que no siempre son evidentes con números crudos.
Una tabla puede resumir, pero una gráfica revela.
</p>

<p style="text-align:justify;">
Un ejemplo clásico de esto es el <strong>Cuarteto de Anscombe</strong>, creado por el estadístico 
<strong>Francis Anscombe (1973)</strong> con el objetivo de demostrar que 
<strong>confiar únicamente en métricas numéricas puede ser engañoso</strong>.
Este cuarteto está compuesto por <strong>cuatro conjuntos de datos distintos</strong> que comparten prácticamente las mismas estadísticas descriptivas:
media, varianza, correlación y hasta la misma recta de regresión lineal.
Sin embargo, cuando se grafican, cada conjunto de datos tiene una 
<strong>distribución completamente diferente</strong>.
</p>

<p style="text-align:justify; font-style:italic;">

<div style="text-align:center; margin-top:1rem; margin-bottom:1rem;">
  <img src="https://github.com/user-attachments/assets/cdfd6142-a459-4ace-883e-3b0c864c30ee"
       alt="Cuarteto de Anscombe"
       width="80%"/>
  <div style="font-size:0.8rem; color:#555;">
    Figura 1. Representación gráfica de los cuatro conjuntos del Cuarteto de Anscombe.  
    Cada gráfico es distinto, aunque las estadísticas básicas son casi idénticas.
  </div>
</div>

<p style="text-align:justify;">
Esto demuestra por qué la visualización es esencial en ciencia de datos, ingeniería, economía, salud, machine learning y prácticamente cualquier área donde se tomen decisiones sobre información.
</p>

<hr/>

<!-- ===================== ESTRUCTURA DEL REPOSITORIO ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">2. Estructura del Repositorio</h2>

<p style="text-align:justify;">
Este repositorio ha sido organizado de acuerdo con los lineamientos de la asignación 
<strong>“Importancia Data Visualization”</strong>. A continuación se describe la función de cada carpeta
y archivo.
</p>

<pre style="background:#f6f8fa; padding:1rem; border:1px solid #d0d7de; border-radius:6px; font-size:0.9rem; line-height:1.4; overflow-x:auto;">
Importancia-Data-Visualization/
│
├── README.md
│        - Documento principal con portada, marco teórico y explicación del trabajo.
│
├── data/
│        - Conjuntos de datos utilizados:
│           - Cuarteto de Anscombe
│           - Datasaurus (13 subconjuntos)
│
├── R/
│        - Scripts en R usados para:
│           - Cargar y mostrar los conjuntos de datos
│           - Graficar cada dataset
│           - Comparar visualmente patrones
│
└── RStudio/   (o el nombre de la herramienta que usaste para la regresión lineal)
         ↳ Código usado para ajuste de regresión lineal
           sobre el subconjunto elegido (por ejemplo "Bullseye"),
           junto con capturas de resultados/gráficos.
</pre>

<hr/>

<!-- ===================== DATA ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">3. Carpeta <code>data/</code></h2>

<p style="text-align:justify;">
En <code>data/</code> se incluyen todos los conjuntos de datos usados en la práctica.
Estos datos son fundamentales porque son la materia prima con la que luego se generan
los análisis y las visualizaciones.
</p>

<ul style="line-height:1.5;">
  <li><strong>Cuarteto de Anscombe:</strong> cuatro archivos (I, II, III y IV) con pares (x,y).</li>
  <li><strong>Datasaurus:</strong> colección de 13 conjuntos de datos con distribuciones visualmente muy diferentes,
      incluso cuando comparten estadísticas similares.</li>
</ul>

<p style="text-align:justify;">
El caso de <strong>Datasaurus</strong> va más allá del ejemplo original de Anscombe. 
Muestra situaciones extremas (por ejemplo, datos que forman la silueta de un dinosaurio, 
un círculo perfecto, una diana tipo “bullseye”, una línea curva, etc.) pero que
numéricamente parecen “normales”.
Esto refuerza la idea de que siempre debemos <strong>ver</strong> los datos, no solo calcularlos.
</p>

<hr/>

<!-- ===================== R ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">4. Carpeta <code>R/</code></h2>

<p style="text-align:justify;">
En esta carpeta se almacenan los scripts en <strong>R</strong> utilizados para:
</p>

<ul style="line-height:1.5;">
  <li>Cargar cada dataset (Anscombe y los 13 del Datasaurus).</li>
  <li>Graficar cada conjunto de puntos en un plano cartesiano (x vs y).</li>
  <li>Observar si la distribución parece lineal, curva, agrupada, con outliers, etc.</li>
  <li>Comparar visualmente por qué datasets con “la misma estadística” NO son iguales realmente.</li>
</ul>

<div style="text-align:center; margin-top:1rem; margin-bottom:1rem;">
  <img src="https://github.com/user-attachments/assets/70500f1b-cbef-4e3b-867a-e1afef119ec5"
       alt="Código R"
       width="60%"/>
  <div style="font-size:0.8rem; color:#555;">
    Figura 2. Ejemplo de script en R usado para cargar y graficar múltiples subconjuntos del Datasaurus.
  </div>
</div>

<p style="text-align:justify;">
El lenguaje R se utiliza porque es una herramienta estándar en análisis estadístico y visualización,
y permite automatizar la generación de gráficos para todos los subconjuntos de datos de manera rápida y reproducible.
</p>

<hr/>

<!-- ===================== REGRESIÓN LINEAL ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">5. Carpeta <code>RStudio/</code> (Regresión lineal)</h2>

<p style="text-align:justify;">
En esta carpeta se documenta el proceso de <strong>regresión lineal</strong> aplicado a uno de los subconjuntos del Datasaurus.
En este caso, el conjunto seleccionado fue <strong>"Bullseye"</strong>.
</p>

<p style="text-align:justify;">
La regresión lineal intenta ajustar una recta que modele la relación entre <code>x</code> y <code>y</code>.
En un escenario idealmente lineal, esa recta tiene sentido para predecir valores.
Sin embargo, "Bullseye" tiene una distribución en forma de diana (círculos concéntricos),
lo cual NO es lineal.
Esto nos permite mostrar un punto muy importante:
<strong>una línea de tendencia puede existir matemáticamente, pero no siempre tiene sentido interpretar esa línea como “explicación del fenómeno”.</strong>
</p>

<div style="text-align:center; margin-top:1rem; margin-bottom:1rem;">
  <img src="https://github.com/user-attachments/assets/c61e6a32-2056-45ee-922d-dae8d4acf581"
       alt="Bullseye dataset"
       width="45%"/>
  <div style="font-size:0.8rem; color:#555;">
    Figura 3. Subconjunto "Bullseye" del Datasaurus.  
    Visualmente es una diana casi perfecta, pero sus métricas resumen parecen normales.
  </div>
</div>

<div style="text-align:center; margin-top:1rem; margin-bottom:1rem;">
  ![graficaMD](https://github.com/user-attachments/assets/09069b2a-f71e-41d5-8fb5-910a04a7716a)
  <div style="font-size:0.8rem; color:#555;">
    Figura 4. Línea Graficada en Clase.  
  </div>
</div>

<p style="text-align:justify;">
Esta parte del trabajo responde a la pregunta:
<strong>¿Qué tan válida es la regresión lineal si la forma real de los datos no es lineal?</strong><br/>
Conclusión: <em>depende de la forma real de los datos, y esa forma solo la ves al graficar.</em>
</p>

<hr/>

<!-- ===================== CONCLUSIONES ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">6. Conclusiones</h2>

<ul style="line-height:1.6; text-align:justify;">
  <li>
    Dos conjuntos de datos pueden “parecer iguales” estadísticamente (misma media, varianza, correlación)
    y aun así ser completamente diferentes en su forma real.
  </li>

  <li>
    Graficar no es opcional: es una parte esencial del análisis, especialmente antes de sacar conclusiones,
    presentar resultados o entrenar modelos.
  </li>

  <li>
    La regresión lineal tiene limitaciones. No basta con dibujar una recta: 
    primero debo validar visualmente si esa recta tiene sentido con la geometría de los datos.
  </li>

  <li>
    Herramientas como R y RStudio permiten automatizar la visualización,
    generando evidencia objetiva (gráficos) que respalda el análisis.
  </li>

  <li>
    La visualización de datos no solo comunica resultados; 
    también <strong>evita malas interpretaciones</strong> y decisiones equivocadas.
  </li>
</ul>

<hr/>

<!-- ===================== REFERENCIAS ===================== -->

<h2 style="color:#003366; margin-top:2rem; margin-bottom:0.5rem;">7. Referencias</h2>

<p style="font-size:0.9rem; text-align:justify;">
Cuarteto de Anscombe. (s/f). <em>Academia-lab.com</em>. Recuperado el 28 de octubre de 2025, de 
https://academia-lab.com/enciclopedia/cuarteto-de-anscombe/
</p>

<br/>
<br/>

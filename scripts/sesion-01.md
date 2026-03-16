# Guion de clase — Sesión 1

## Sesión

**Título:** Sesión 1: ¿Qué es la IA y dónde está en tu vida?  
**Duración sugerida:** 40–45 minutos  
**Público:** estudiantes de preparatoria, 15–18 años, México  
**Objetivo central:** que el grupo se lleve una idea muy concreta: en su forma más simple, el machine learning puede empezar con matemáticas que ya conocen, especialmente la recta `y = mx + b`.

---

## Nota para quien imparte

Este guion está escrito para sonar oral, no académico. La meta no es leerlo palabra por palabra de forma rígida, sino usarlo como base.  

Usa estas marcas:

- `[Pausa]` para dejar que una idea caiga.
- `[Pregunta al grupo]` para invitar participación.
- `[Mostrar animación]` para activar un recurso de la sesión.
- `[Si falla la animación]` para improvisar con pizarrón o explicación verbal.
- `[Tono]` para sugerir la energía del momento.

---

## Apertura

### 0. Bienvenida

Buenos días, buenas tardes. Hoy vamos a empezar un curso sobre inteligencia artificial, pero no lo vamos a empezar con robots, ni con películas de ciencia ficción, ni con palabras rarísimas.

Lo vamos a empezar con algo mucho más cercano: las apps que ustedes ya usan todos los días, y una idea de matemáticas que ya conocen desde hace tiempo.  

[Pausa]

La meta de hoy es que salgan pensando esto:

**“La IA no es magia. Y una parte del machine learning empieza con una recta.”**

[Pausa breve]

Si al final de la sesión esa idea les queda clara, la sesión ya cumplió su objetivo.

---

## 1. Hook con TikTok

### 1.1 Inicio fuerte

[Tono: directo, rápido]

Abre TikTok ahora mismo en tu cabeza. No hace falta sacar el celular. Solo piensa en esto:

el primer video que ves, el primer audio que escuchas, el primer contenido que te aparece, no lo eligió una persona. No hay un editor sentado diciendo “a Michelle le voy a poner este video, a Diego este otro”.

Lo decidió un sistema.

Un algoritmo.

Una inteligencia artificial.

[Pausa]

Y lo impresionante es que esa decisión ocurre en segundos, usando señales sobre tu comportamiento: cuánto tiempo te quedas viendo un video, si lo repites, si lo compartes, si te lo saltas muy rápido.

[Pregunta al grupo]
¿Quién de aquí siente que TikTok “ya lo conoce demasiado bien”?

[Deja que levanten la mano o respondan]

Exacto. Esa sensación de “me conoce” no significa que te lea la mente. Significa que detecta patrones.

### 1.2 Animación de TikTok

[Mostrar animación de TikTok]

Aquí quiero que observen algo: el sistema no empieza con un solo video. Empieza con varios candidatos. Los compara. Les asigna una puntuación. Y luego los ordena.

[Pausa]

Lo importante no es memorizar los números. Lo importante es entender la lógica:

**señales de comportamiento -> puntuación -> ranking -> contenido que aparece primero**

[Si falla la animación]
Dibuja cuatro rectángulos en el pizarrón, escribe arriba de cada uno un tipo de video, y debajo anota señales como “tiempo de visualización”, “repeticiones” y “compartidos”. Luego explica que el algoritmo ordena según esa información.

### 1.3 Cierre del hook

TikTok no está solo.

Spotify recomienda música.  
Google Maps predice tráfico.  
Gmail decide qué correo mandar a spam.  
Instagram detecta tu cara para ponerte filtros.

Vivimos rodeados de IA.

Pero aquí viene el problema: muchas personas usan IA todos los días sin tener idea de qué está pasando por debajo.

Y cuando no entiendes el mecanismo, todo parece magia.

---

## 2. Lo que la IA no es

[Tono: calmado, desmitificador]

Entonces empecemos rompiendo una idea falsa.

La IA no es magia.

No es una mente consciente.
No es un robot con deseos propios.
No es algo que “entiende” el mundo exactamente como lo entiendes tú.

[Pausa]

En el fondo, la IA es una combinación de:

- datos,
- matemáticas,
- y reglas o modelos para detectar patrones.

Eso no la hace menos impresionante. La hace más interesante.

Porque si entiendes el mecanismo, ya no te intimida tanto.  
La puedes cuestionar.  
La puedes usar con más criterio.  
Y también puedes detectar cuándo se equivoca.

---

## 3. El giro de la sesión

[Tono: revelación]

Y aquí viene la sorpresa importante de hoy.

Si alguna vez viste en álgebra la fórmula de la recta:

`y = mx + b`

entonces ya viste una de las ideas más simples del machine learning.

[Pausa larga]

Sí. Así de simple.

Antes de modelos gigantes, antes de ChatGPT, antes de palabras complicadas, hay una idea muy básica:

**encontrar una relación entre dos cosas.**

Por ejemplo:

- horas de estudio
- y calificación

Si una sube, la otra tiende a subir también.

Y una forma muy simple de representar esa relación es con una recta.

[Pregunta al grupo]
Si una persona estudia más horas, en general, ¿qué esperarían que pase con su calificación?

[Escucha respuestas]

Exacto: no siempre, no perfectamente, pero en general esperaríamos que suba.

Y ahora viene lo importante:

cuando hablamos de “aprendizaje” en machine learning, aquí no significa pensar ni sentir.

Significa algo mucho más concreto:

**encontrar los números correctos para la recta.**

### 3.1 Explicación de m y b

Aquí aparecen dos protagonistas:

- `m`, la pendiente
- `b`, la intersección con el eje y

`m` nos dice cuánto sube la recta por cada paso a la derecha.  
`b` nos dice dónde empieza la recta cuando `x = 0`.

[Pausa]

O dicho en una frase más cotidiana:

**sube sobre avanza**

o, si quieren verlo en inglés porque también lo van a encontrar así:

**rise over run**

---

## 4. Reto principal: antes que la máquina

[Tono: participativo]

Ahora no quiero que solo me escuchen. Quiero que intenten hacer ustedes el trabajo primero.

Vamos a usar una gráfica con estudiantes y sus horas de estudio.  
Cada punto azul representa un dato real.  
Y ustedes van a mover una recta para tratar de ajustarla lo mejor posible.

### 4.1 Presentación del reto

[Mostrar animación / demo de regresión]

Aquí lo importante no es adivinar una “respuesta secreta”.  
Lo importante es probar una hipótesis:

“Creo que la relación entre horas de estudio y calificación se ve más o menos así.”

[Pausa]

### 4.2 Guía oral durante el ajuste manual

Primero, fíjense en la pendiente.

[Señala `m`]

Si la pendiente es muy pequeña, la recta queda muy plana.  
Si es demasiado grande, la recta sube demasiado rápido.

Ahora fíjense en `b`.

[Señala `b`]

Si `b` está muy arriba o muy abajo, la recta arranca en un lugar incorrecto.

[Pregunta al grupo]
¿Qué conviene mover primero: la pendiente o la intersección?

[Escucha 2 o 3 respuestas]

No hay una única estrategia, pero mucha gente primero ajusta la inclinación general y luego el punto de arranque.

### 4.3 El momento pedagógico clave

[Tono: enfático]

Aquí está el corazón de toda la sesión:

**esto ya es machine learning en miniatura.**

¿Por qué?

Porque estamos:

1. viendo datos,
2. proponiendo un modelo,
3. midiendo error,
4. y ajustando para reducir ese error.

[Pausa]

Eso es exactamente la lógica básica del aprendizaje.

No hay magia.

Hay datos, una hipótesis matemática y una forma de medir qué tan mal o qué tan bien va esa hipótesis.

### 4.4 Rise over run

[Señala el triángulo o indicación visual de la pendiente]

Quiero que miren esta parte con cuidado.

Cuando avanzamos 1 hora a la derecha, la recta sube cierta cantidad de puntos.

Eso es la pendiente.

Si avanza 1 y sube 5, la pendiente es 5.  
Si avanza 1 y sube 2, la pendiente es 2.

[Pausa]

Entonces cuando una máquina “aprende” esta recta, en esta versión tan simple, lo que realmente está aprendiendo es:

**cuánto conviene que suba la recta y desde dónde conviene arrancarla.**

### 4.5 Entrega a la máquina

[Mostrar botón: “Ahora deja que la máquina aprenda”]

Ahora sí, dejen que la máquina haga el ajuste.

[Pausa mientras corre la animación]

Quiero que observen esto:

- aparecen los errores,
- la recta se mueve,
- y termina en una versión que resume mejor la tendencia general.

[Pausa]

Y otra vez: el punto no es que la recta pase por todos los puntos.  
El punto es que capture bien el patrón general.

### 4.6 Predicción final

Ahora, ya con la recta ajustada, podemos preguntar:

si una persona estudia cierta cantidad de horas, ¿qué calificación aproximada esperaríamos?

Eso ya es una predicción.

Y aquí pueden decir una frase muy importante:

**la máquina no vio ese caso exacto, pero usa el patrón que aprendió para estimarlo.**

[Si falla la animación]
Dibuja unos 6–8 puntos en el pizarrón, traza una recta aproximada y pregunta al grupo dónde debería quedar para “equivocarse menos”. Luego marca una predicción en un valor nuevo de `x`.

---

## 5. Poner nombre a lo que acaban de hacer

[Tono: ordenando ideas]

Lo que acabamos de ver tiene nombre:

**aprendizaje supervisado**

Supervisado significa que sí conocemos las respuestas correctas de los ejemplos de entrenamiento.

En nuestro caso:

- entrada: horas de estudio
- salida correcta: calificación real

La máquina usa esos ejemplos para aprender una relación.

Dentro del aprendizaje supervisado hay dos familias muy comunes:

- **regresión**, cuando predices un número
- **clasificación**, cuando predices una categoría

### 5.1 Ejemplos rápidos

Regresión:

- precio de una casa,
- tiempo de llegada de un viaje,
- consumo de energía mañana.

Clasificación:

- spam o no spam,
- tumor o no tumor,
- eres tú o no eres tú en reconocimiento facial.

[Pausa]

Así que ya no piensen “machine learning” como algo abstracto.  
Piénsenlo también como:

**ajustar modelos para hacer predicciones a partir de datos.**

---

## 6. IA, Machine Learning y Deep Learning

[Tono: ordenar términos]

Ahora sí podemos poner orden en tres palabras que escuchan muchísimo:

- inteligencia artificial,
- machine learning,
- deep learning.

[Mostrar mapa conceptual]

Quiero que lo lean como capas anidadas.

### 6.1 Explicación oral

La más grande es **Inteligencia Artificial**.

Ese es el campo amplio: cualquier sistema diseñado para realizar tareas que asociamos con inteligencia.

Dentro de eso está **Machine Learning**.

Aquí entran los sistemas que aprenden patrones a partir de datos.

Y dentro de machine learning está **Deep Learning**.

Eso ya se refiere a redes neuronales con muchas capas, que son las que han impulsado muchos avances recientes en texto, imagen y voz.

[Pausa]

Entonces la frase corta es:

**deep learning vive dentro de machine learning, y machine learning vive dentro de IA.**

### 6.2 Conectar con lo anterior

Lo importante es que la recta que acabamos de ver ya estaba en la parte de machine learning.

No hacía falta empezar con algo enorme para entrar en el tema.

---

## 7. Recorrido de apps

[Tono: dinámico]

Ahora regresamos a las apps del principio, pero con una mirada más inteligente.

[Mostrar recorrido de apps]

Aquí no quiero que memoricen marcas. Quiero que se hagan una sola pregunta:

**¿qué problema está resolviendo la IA en cada caso?**

### 7.1 TikTok

En TikTok, la tarea principal es **ranking**: ordenar qué contenido mostrar primero.

### 7.2 Spotify

En Spotify, la tarea es **recomendación**: sugerir música según patrones de audio y de comportamiento.

### 7.3 Google Maps

En Maps, la tarea es **predicción**: estimar tráfico y tiempo de llegada.

### 7.4 Instagram

En Instagram, la tarea es **visión por computadora**: detectar rasgos y posiciones de una cara.

### 7.5 Gmail

En Gmail, la tarea es **clasificación**: decidir si un correo es spam o no.

### 7.6 DiDi / Uber

En DiDi o Uber, la tarea es **optimización y predicción**: estimar demanda, tiempo, precio y rutas.

[Pausa]

La idea importante aquí es:

**la IA no es una sola cosa. Es una familia de técnicas aplicadas a problemas distintos.**

---

## 8. Los otros dos paradigmas

### 8.1 Aprendizaje no supervisado

[Tono: exploratorio]

Ahora imaginen que ya no tenemos respuestas correctas.

Solo tenemos datos.

Por ejemplo: canciones con ciertas características, pero sin etiquetas de género.

Le pedimos a la máquina que agrupe cosas parecidas.

Eso es **aprendizaje no supervisado**.

[Mostrar animación de K-means]

Aquí el algoritmo no recibe la respuesta correcta.  
Solo recibe puntos y busca estructura.

La idea más importante que quiero que digan aquí es:

**el algoritmo encuentra grupos; el nombre del grupo lo ponemos nosotros después.**

[Pausa]

Eso evita una confusión muy común.

### 8.2 Aprendizaje por refuerzo

Ahora imaginen otro caso.

No hay una lista de respuestas correctas, pero sí hay premios y castigos.

Pruebo una acción.  
Me va bien o me va mal.  
Ajusto.  
Intento otra vez.

Eso es **aprendizaje por refuerzo**.

[Mostrar animación de RL]

Aquí el agente aprende por experiencia:

- estado,
- acción,
- recompensa,
- ajuste de estrategia.

La frase clave aquí es:

**aprender por refuerzo es mejorar una estrategia a partir de prueba, error y recompensa.**

---

## 9. Actividad final: Teachable Machine

[Tono: invitación práctica]

Hasta aquí hemos entendido ideas.

Ahora quiero que vean que también se puede construir algo sencillo.

Teachable Machine permite entrenar un modelo básico sin programar.

Aquí puedes decir:

“No hace falta que hoy memoricen todos los pasos. Lo importante es que vean que un modelo necesita ejemplos para aprender.”

### 9.1 Mientras explicas la actividad

Subraya tres ideas:

1. si das pocos ejemplos, el modelo se confunde,
2. si los ejemplos son muy parecidos entre sí, el modelo no generaliza bien,
3. los datos de entrenamiento importan muchísimo.

[Pausa]

Eso conecta perfecto con todo lo que vimos hoy:

la IA aprende de patrones,
pero depende de los datos que recibe.

---

## 10. Cierre

[Tono: claro, memorable]

Si hoy se quedaran con una sola idea, me gustaría que fuera esta:

La inteligencia artificial no es magia.

Y, en su versión más simple, el machine learning puede empezar con algo que ustedes ya conocían:

**una recta, una pendiente, una intersección y un error que se intenta reducir.**

[Pausa larga]

Eso cambia por completo la manera de ver el tema.

Porque cuando entiendes eso, la IA deja de verse como truco y empieza a verse como matemáticas aplicadas a reconocer patrones.

### 10.1 Última pregunta al grupo

[Pregunta al grupo]
¿Qué les sorprendió más hoy: que ya usaban IA diario, o que una parte del machine learning empieza con álgebra básica?

[Escucha algunas respuestas]

Excelente. Esa era justo la idea.

Nos vemos en la siguiente sesión.

---

## Apéndice: recursos de apoyo para quien imparte

### Si quieres reforzar la idea central

Puedes repetir alguna de estas frases a lo largo de la sesión:

- “La IA más simple empieza con una recta.”
- “Aquí aprender no significa pensar; significa ajustar números.”
- “Machine learning no siempre empieza con algo futurista. A veces empieza con álgebra.”
- “Datos + error + ajuste = una de las bases del aprendizaje automático.”

### Si el grupo está muy participativo

Haz estas preguntas extra:

- “¿Qué app creen que usa más IA en su vida diaria?”
- “¿En qué momento una recomendación deja de ser casual y empieza a ser algorítmica?”
- “¿Qué creen que pasaría si entrenáramos un modelo con datos malos?”

### Si el grupo está callado

Usa preguntas de respuesta corta:

- “¿Sube o baja?”
- “¿Número o categoría?”
- “¿Hay respuesta correcta o no?”
- “¿Premio/castigo o ejemplos etiquetados?”

### Si falla toda la parte interactiva

La sesión sigue funcionando si haces tres cosas en el pizarrón:

1. Dibujar una tabla simple de horas de estudio y calificación.
2. Colocar puntos en un plano cartesiano.
3. Trazar dos o tres rectas posibles y preguntar cuál se ajusta mejor.

Con eso, la idea pedagógica central sigue intacta.

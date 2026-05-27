# ¿Confían realmente los desarrolladores en la inteligencia artificial?

![AI Sentiment Distribution](images/ai_sentiment_distribution.png)

La inteligencia artificial ya forma parte del día a día de muchos desarrolladores, pero una pregunta sigue siendo clave: **¿realmente confían los programadores en estas herramientas?**

Para responderla, analicé la **Stack Overflow Developer Survey 2024**, una encuesta global sobre perfiles, experiencia, herramientas y percepción de la IA en el desarrollo de software. La versión utilizada procede del dataset preparado por TidyTuesday, que contiene respuestas codificadas y listas para trabajar con análisis tabular y machine learning.

El análisis se centró en cinco preguntas principales:

1. ¿Cómo se distribuye el sentimiento hacia la IA entre los desarrolladores?
2. ¿Influye la experiencia programando en esa percepción?
3. ¿Está relacionada la confianza en la precisión de la IA con una opinión positiva?
4. ¿Qué variables ayudan más a predecir el sentimiento hacia la IA?
5. ¿Qué ocurriría en un escenario predictivo con un perfil hipotético de desarrollador?

Los resultados muestran que el sentimiento positivo hacia la IA es el patrón dominante. Sin embargo, la confianza parece ser un factor clave: los desarrolladores que confían más en la precisión de las herramientas de IA tienden a mostrar una actitud más favorable. La experiencia programando también aporta contexto, aunque no explica por sí sola la percepción hacia la IA.

Para completar el análisis, entrené un modelo **Random Forest** que agrupa el sentimiento en tres categorías: **Negative**, **Neutral / Unsure** y **Positive**. El modelo alcanzó una accuracy aproximada del **68.65%**, con una balanced accuracy del **49.11%**, un macro F1-score de **0.50** y un weighted F1-score de **0.68**.

Estos resultados indican que el modelo identifica bastante bien el sentimiento positivo, pero tiene más dificultad con opiniones negativas o neutrales. Esto ocurre porque el dataset está desbalanceado: hay muchas más respuestas positivas que negativas o inciertas.

La conclusión principal es clara: **la comunidad desarrolladora muestra una señal positiva hacia la IA, pero esa aceptación depende fuertemente de la confianza**. Usar IA no significa necesariamente confiar plenamente en ella; la percepción sobre su precisión, su capacidad para resolver tareas complejas y su impacto laboral siguen siendo factores decisivos.

## ¿Qué podemos aprender de esto? Recomendaciones

1. **Para creadores de herramientas de IA:** la confianza debe ser una prioridad. No basta con generar respuestas rápidas; las herramientas deben explicar mejor sus sugerencias, reducir errores y facilitar que el desarrollador entienda por qué una recomendación es válida.

2. **Para equipos de desarrollo:** el código generado por IA debería revisarse sistemáticamente antes de integrarse en producción. La IA puede acelerar tareas, pero la responsabilidad final debe seguir estando en procesos de revisión, pruebas y validación humana.

3. **Para empresas que adoptan IA:** la formación es clave. Los equipos necesitan aprender cuándo confiar en una herramienta de IA, cuándo cuestionarla y cómo combinarla con buenas prácticas de ingeniería de software.

En resumen, la IA ya no es solo una promesa futura para los desarrolladores: es una herramienta presente. Pero su adopción real dependerá de algo más humano que técnico: la confianza.
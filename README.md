# Proyecto: Análisis Comparativo del Impacto Ambiental entre la medición de Hardware con CarbonTracker y Análisis de Ciclos de vida con openLCA

**[CarbonTracker](https://github.com/lfwa/carbontracker)** se usó componente activo que permite realizar proyecciones detalladas y con datos en tiempo real del consumo energético y la huella de carbono generada por algoritmos intensivos en cómputo. Está diseñado para ser utilizado en contextos científicos, como la biología computacional, donde la evaluación de la sostenibilidad computacional es clave para avanzar hacia una ciencia responsable.

---

## Características Principales

- Entrenamiento simulado de modelos de Deep Learning en PyTorch con registro de consumo por época (batch) usando CarbonTracker
- Proyección geográfica personalizada: compara el impacto si la misma tarea se ejecutara en países como Alemania, China, Singapur, Finlandia, etc.
- Estimación de huella de carbono (gCO₂eq/kWh) combinando intensidad de red y eficiencia del centro de datos
- Visualización automática con gráficos estilizados y exportación de resultados en .csv
- Capacidad multiescenario y replicabilidad

---

## Propósito

Es script permite al usuario: 
- Medir el consumo energético directo del hardware (TI) usando CarbonTracker.
- Proyectar el impacto ambiental de dicha carga de trabajo en distintos paises y centros de datos.
- Visualizar la evolución energética por épocas y comparar resultados entre escenarios.
- Apoyar la toma de decisiones sobre sostenibilidad en investigación computacional intensiva.

---

## Funcionalidades Principales

1. **Medición base de TI:** Calcula el consumo de energía y carbono en el hardware Local.
2. **Proyección por escenarios:** Evalúa el impacto si la tarea se ejecutará en paises con diferentes PUE e intensidad de carbono.
3. **Visualización automática:** Genera Múltiples gráficos comparativos (barras, lineas, agrupados).
4. **Salida CSV:** Archivos detallados con varibales calve por país y época.
5. **Ranking Global:** Clasifica países po su intensidad de carbono proyectada.

--

## Estructura de Salida

Tras la ejecución, se genera: 
- consolidated_carbon_tracking_results.csv: resumen por país y época.
- *.png: gráficos de comparación energética y de huella de carbono.
- base_it_tracking_logs/: logs de CarbonTracker por época.


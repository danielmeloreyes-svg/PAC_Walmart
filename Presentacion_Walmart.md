# Análisis de Ventas Walmart
## Predicción de Ventas Semanales

---

## Introducción

**Caso de Estudio: Walmart Store Sales Forecasting**

- **Fuente**: Competencia de Kaggle - Walmart Recruiting Store Sales Forecasting
- **Objetivo**: Desarrollar un modelo predictivo para ventas semanales
- **Alcance**: 45 tiendas, múltiples departamentos, datos históricos 2010-2012
- **Relevancia**: Optimización de inventario y planificación estratégica

---

## Descripción del Problema

### Contexto Empresarial
- Walmart necesita predecir ventas semanales por tienda y departamento
- **Desafío**: Variabilidad en ventas debido a múltiples factores externos
- **Impacto**: Decisiones de inventario, personal y promociones

### Variables Clave
- **Ventas semanales** (variable objetivo)
- **Factores externos**: Temperatura, precio combustible, desempleo, CPI
- **Promociones**: 5 tipos de MarkDowns
- **Características de tienda**: Tipo (A/B/C), tamaño, ubicación

---

## Objetivos

### Objetivo General
Desarrollar un análisis estadístico completo para la predicción de ventas semanales de Walmart

### Objetivos Específicos
1. **Preprocesar** datos para garantizar calidad y consistencia
2. **Construir indicadores** de rendimiento y estacionalidad
3. **Identificar patrones** en el comportamiento de ventas
4. **Evaluar impacto** de promociones y factores externos
5. **Proporcionar insights** para la toma de decisiones

---

## Carga de Datos

### Fuentes de Información
- **train.csv**: 421,570 registros de ventas históricas
- **features.csv**: Variables externas (temperatura, promociones, etc.)
- **stores.csv**: Características de las 45 tiendas

### Estructura de Datos
```
• Período: 2010-2012
• Tiendas: 45 (Tipos A, B, C)
• Departamentos: Múltiples por tienda
• Frecuencia: Semanal
• Variables: 15+ características
```

---

## Preprocesamiento de Datos

### 1. Limpieza de Datos Faltantes
- **Problema**: Valores NA en variables MarkDown (promociones)
- **Solución**: Reemplazo con 0 (ausencia de promoción)
- **Resultado**: 100% de completitud en variables clave

### 2. Detección de Outliers
- **Método**: Análisis IQR para ventas semanales
- **Hallazgo**: Identificación de valores extremos
- **Tratamiento**: Documentación para análisis posterior

### 3. Transformación de Variables
- **Total_MarkDown**: Suma de todas las promociones
- **Season**: Categorización estacional (Invierno, Primavera, Verano, Otoño)
- **Variables temporales**: Año y mes extraídos de fechas

---

## Construcción de Indicadores

### 1. Rendimiento por Tienda
- **Ventas totales y promedio** por tienda
- **Ranking** de tiendas por desempeño
- **Identificación** de tiendas top performers

### 2. Análisis de Estacionalidad
- **Patrones mensuales** de ventas
- **Comparación estacional** (Invierno vs Verano)
- **Identificación** de períodos de mayor/menor demanda

### 3. Impacto de Promociones
- **Comparación** ventas con/sin promociones
- **Cálculo de incremento** porcentual por promociones
- **Efectividad** de estrategias de descuento

### 4. KPIs por Tipo de Tienda
- **Ventas promedio** por tipo (A, B, C)
- **Número de tiendas** por categoría
- **Análisis comparativo** de rendimiento

---

## Resultados Principales

### Hallazgos Clave
- **Estacionalidad**: Patrones claros de demanda por estación
- **Promociones**: Impacto positivo medible en ventas
- **Diferencias por tipo**: Rendimiento variable según categoría de tienda
- **Outliers**: Presencia de valores extremos que requieren atención

### Indicadores Generados
- ✅ **15+ métricas** de rendimiento por tienda
- ✅ **Análisis estacional** completo
- ✅ **Evaluación de promociones** cuantificada
- ✅ **KPIs comparativos** por tipo de tienda

---

## Conclusiones y Recomendaciones

### Conclusiones
1. **Datos preparados** para modelado estadístico avanzado
2. **Indicadores robustos** para monitoreo de rendimiento
3. **Patrones identificados** en comportamiento de ventas
4. **Base sólida** para predicciones futuras

### Recomendaciones
- **Implementar** monitoreo continuo de indicadores
- **Optimizar** estrategias promocionales basadas en hallazgos
- **Considerar** estacionalidad en planificación de inventario
- **Profundizar** análisis de tiendas con rendimiento atípico

---

## Próximos Pasos

### Desarrollo del Modelo
- **Modelado estadístico** descriptivo e inferencial
- **Análisis de correlaciones** entre variables
- **Modelos de regresión** para predicción
- **Validación** y testing del modelo final

### Implementación
- **Dashboard** de monitoreo en tiempo real
- **Alertas automáticas** para valores atípicos
- **Integración** con sistemas de inventario
- **Capacitación** del equipo en interpretación de resultados

---

## Agradecimientos

**Análisis desarrollado para el curso de Estadística**

*Maestría en Ciencia de Datos*

**Herramientas utilizadas:**
- R, R Markdown
- Librerías: readr, dplyr, ggplot2
- Metodología estadística aplicada

---

## Preguntas y Discusión

**¿Alguna pregunta sobre el análisis realizado?**

**Contacto:** [Tu información de contacto]

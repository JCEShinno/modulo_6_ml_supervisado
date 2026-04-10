# Proyecto Módulo 6 - Aprendizaje de Máquina Supervisado

## Descripción
Proyecto de machine learning supervisado aplicado a un problema de e-commerce. El objetivo consiste en predecir el monto promedio de compra esperado de un cliente a partir de variables demográficas, de navegación y de comportamiento comercial. El trabajo incluye generación y preparación del dataset, validación cruzada, comparación de algoritmos, optimización y selección de un modelo final.

## Objetivo
Diseñar e implementar un modelo predictivo de regresión que permita estimar el monto promedio de compra de un cliente, con el fin de apoyar estrategias de personalización comercial y optimización de campañas de marketing.

## Tecnologías utilizadas
- Python
- Pandas
- NumPy
- scikit-learn
- Matplotlib

## Estructura del proyecto
- `data/raw/`: dataset base del proyecto
- `data/interim/`: archivos intermedios del flujo de modelado
- `data/processed/`: archivos procesados si corresponde
- `notebooks/`: notebook principal del proyecto
- `outputs/`: visualizaciones de métricas y resultados
- `docs/`: informe final técnico
- `README.md`: descripción general del repositorio

## Desarrollo del proyecto
El notebook principal se organiza en ocho etapas:

1. Fundamentos del aprendizaje de máquina  
2. Nivel de ajuste del modelo y validación cruzada  
3. Preprocesamiento y escalamiento de datos  
4. Regresiones  
5. Algoritmos de clasificación  
6. Métricas de desempeño  
7. Optimización del modelo  
8. Algoritmos de Boosting  

## Modelos trabajados
- Regresión lineal
- Regresión polinomial
- KNN Classifier (como contraste conceptual)
- KNN Regressor
- Ridge
- Lasso
- Gradient Boosting Regressor

## Principales hallazgos
- El problema fue correctamente abordado como una tarea de regresión supervisada.
- La regresión polinomial mejoró el desempeño de la regresión lineal base.
- KNN Regressor obtuvo un desempeño intermedio respecto de los modelos lineales y no lineales.
- Ridge y Lasso aportaron estabilidad, pero no superaron a los mejores modelos no lineales.
- Gradient Boosting obtuvo el mejor desempeño final del proyecto.
- Las variables con mayor peso predictivo fueron principalmente `visitas_sitio_mes`, `engagement_total`, `score_fidelizacion`, `paginas_por_visita` y `tiempo_promedio_sitio_min`.

## Resultados finales
Comparación final de modelos en conjunto de prueba:

- **Gradient Boosting**: RMSE = 12708.2660 | R² = 0.7254  
- **Regresión polinomial**: RMSE = 12744.3727 | R² = 0.7239  
- **KNN Regressor optimizado**: RMSE = 13536.7664 | R² = 0.6884  
- **Ridge (lineal optimizado)**: RMSE = 13745.2054 | R² = 0.6788  

## Archivos principales
- `notebooks/proyecto_modulo_6_ml_supervisado.ipynb`
- `data/raw/clientes_ecommerce_ml_raw.csv`
- `data/interim/clientes_ecommerce_ml_limpio.csv`
- `data/interim/resumen_outliers_ml.csv`
- `outputs/` con visualizaciones de métricas y comparación de modelos
- `docs/informe_final_modulo_6_ml.pdf`

## Conclusión
El proyecto permitió implementar un pipeline completo de aprendizaje supervisado de punta a punta, comparando distintos algoritmos y seleccionando un modelo final con base en métricas objetivas de desempeño. Gradient Boosting fue elegido como la mejor alternativa final por su mejor equilibrio entre error predictivo y capacidad explicativa.

## Autor
Juan Carlos Castro Encina

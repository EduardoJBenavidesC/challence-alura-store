# Challenge: Alura Store - Especialización Data Science
> **Análisis de Eficiencia Operativa para la Toma de Decisiones Estratégicas**

<br>

## 1. Contexto del Proyecto
Este proyecto tiene como objetivo asesorar a la dirección en la toma de decisiones estratégicas para su cadena de tiendas, evaluando
el desempeño de 4 unidades de negocio basándose en indicadores reales de ventas, satisfacción del cliente y eficiencia logística.

---

## 2. Metodología y Arquitectura de Datos
Para garantizar la fiabilidad de los resultados, se implementó un flujo de trabajo en el **entorno de ejecución (Cloud Environment) Google Colab**, 
utilizando Python como motor de procesamiento.

### Fases del Proceso:
1. **Carga y Auditoría de Estructura:** Importación de fuentes externas vía GitHub y validación de dimensiones de datos.
2. **Data Quality:** Limpieza de duplicados, gestión de nulos y validación de reglas de negocio (ej. Precios ≥ 0).
3. **Persistencia en Nube:** Integración con Google Drive para el respaldo automático de resultados.

---

## 3. Protocolo de Almacenamiento y Respaldo
El sistema está diseñado para centralizar los resultados en una ubicación fija dentro del ambiente **Google Colab**.

> [!CAUTION]
> **PUNTO DE CONTROL: Validación de Ruta**
> En la cuarta celda, el sistema ejecuta una rutina de verificación mediante `os.path.exists`. 
> * **Si recibe un mensaje de ALERTA:** Significa que el directorio **AluraStore** no ha sido detectado en su unidad de Drive.
> * **Acción Requerida:** Debe crear la carpeta manualmente o ajustar la variable `ruta_proyecto` **antes** de proceder a las celdas de exportación.


---

## 4. Estándar de Resultados (Output)
Cada análisis genera dos archivos .csv complementarios.
Esta duplicidad es técnica fue desdarrollada para evitar que las etiquetas del reporte (tal como se muestra en los diplay) ensucien los cálculos de los gráficos.

| Tipo de Archivo | Propósito | Características Técnicas |
| :--- | :--- | :--- |
| **DATA** | Para análisis o uso posterior | Formato Raw, sin índices, codificación UTF-8-SIG. |
| **REPORTE** | Informe de Resultados | Formato Raw, sin índices, listo para interpretación. |

**Nota técnica:** Ambas versiones se exportan **sin índices y sin formato visual**, asegurando archivos ligeros, técnicos y compatibles con cualquier herramienta de inteligencia de negocios.

---

## 5. Conclusiones: "Cuando el volumen no compra la rentabilidad"

Tras el procesamiento integral de los datos, el diagnóstico técnico identifica a la **Tienda 4** como la unidad con menor eficiencia estratégica. Los hallazgos confirman una desconexión crítica entre el esfuerzo operativo y la captura de valor:

* **Erosión de Ingresos:** En categorías core como *Electrónicos*, la sucursal moviliza un volumen de unidades similar a la líder, pero genera un **70% menos de ingresos**.
* **Baja Captura de Valor:** La unidad sostiene una brecha negativa de ingresos del 10% respecto a la red, explicada por el ticket promedio más bajo en el 75% de su operación.
* **Falla de Ejecución:** Dado que el perfil de demanda es homogéneo en toda la cadena (90% de coincidencia), el bajo desempeño puede obeder a factores de gestión interna.

> [!IMPORTANT]
> **RECOMENDACIÓN ESTRATÉGICA**
> Basado en la evidencia técnica, se dictamina la **desinversión de la Tienda 4**. Esta acción permitirá optimizar el capital del Sr. Juan, redirigiendo los recursos hacia unidades con mayor capacidad de generación de rentabilidad y valor.

<br>

---
<p align="center">
  <b>Especialización en Data Science - Challenge Alura Store</b><br>
  <i>Análisis de datos para la toma de decisiones estratégicas.</i>
</p>
  


# Diseño de Redes de Atraso 

El diseño de redes de atraso es una técnica crucial en el control digital que se basa en la manipulación de las respuestas en frecuencia de un sistema. Este tipo de diseño permite ajustar la estabilidad y el rendimiento del sistema, minimizando problemas como el ruido o los errores en estado estacionario. A través del análisis del diagrama de Bode, se pueden identificar los márgenes de ganancia y fase, y determinar las modificaciones necesarias para cumplir con los requisitos de estabilidad y velocidad de respuesta.


## 1.Controladores por Análisi en Frecuencia

Los controladores diseñados mediante análisis en frecuencia se emplean en aplicaciones donde es importante ajustar el margen de fase y ganancia para mantener el sistema estable. Un controlador PID, por ejemplo, es una combinación de redes de adelanto y atraso que afecta tanto las respuestas en baja como en alta frecuencia.

>🔑 *Controlador PID:* Un controlador que combina acciones proporcionales, integrales y derivativas para mejorar la estabilidad y el tiempo de respuesta de un sistema.

### 1.1.Redes de adelanto de fase

La compensación por adelanto de fase mejora significativamente la respuesta transitoria del sistema, lo que permite una mayor velocidad de respuesta y un incremento en el ancho de banda y los márgenes de estabilidad. Sin embargo, este tipo de compensación también tiene el inconveniente de amplificar el ruido en altas frecuencias debido al aumento de la ganancia en esas bandas, lo que puede afectar el rendimiento general del sistema.

### 1.2.Redes de atraso de fase

La compensación por atraso de fase disminuye la ganancia en altas frecuencias sin afectar las bajas, lo que reduce el ancho de banda del sistema y, en consecuencia, disminuye su velocidad. Sin embargo, esta compensación mejora notablemente la precisión en estado estacionario y suprime eficazmente el ruido en frecuencias altas, aunque esto ocurre a costa de un mayor tiempo de respuesta transitoria.

### 1.3.Redes de Atraso - Adelante de fase

El compensador de atraso-adelanto integra los beneficios de ambos tipos de compensación, lo que facilita la mejora en los márgenes de estabilidad, el aumento del ancho de banda y la disminución del error en estado estacionario, todo sin incrementar el ruido. No obstante, este tipo de compensador aumenta el orden del sistema en dos niveles, lo que añade complejidad y dificulta el control de la respuesta transitoria, a diferencia de los compensadores de atraso o adelanto individuales, que solo incrementan el orden en uno.

## 2.Margenes de Fase y Ganancia

### 2.1.Margen de Ganancia

 * Es el cambio en la ganancia de lazo abierto de un sistema que se requerie para que el Sistema en lazo cerrado sea inestable,
 * Esta parte se mide en decibeles(dB)
 * Se mide tomando como referencia la fase de -180°
 * Ayuda a definir la estabilidad del sistema

### 2.2.Margen de Fase

 * Es el cambio en la fase de lazo abierto, requerido para que el Sistema en lazo cerrado sea inestable
 * Se mide en grados(°)
 * Se toma como referencia de medida la ganancia unitario (0dB)
 * MP > −180° Positivo o MP < −180° Negativo

### 2.3.Medida de Margenes de Estabilidad

![MGP](Redes-de-Atraso/MGP.png)


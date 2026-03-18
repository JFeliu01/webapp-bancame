# 1. Conceptualización y Definición del Problema

## Resumen Ejecutivo
El problema central de banca.me es la insostenibilidad de su proceso manual para otorgar créditos ante el crecimiento explosivo de la demanda,
lo que genera un cuello de botella operativo. Para resolverlo, se desarrollará una aplicación web de autoservicio que automatice la captura de datos financieros,
la evaluación de riesgo crediticio básica y la generación de contratos digitales, eliminando la necesidad de contactos iniciales.
Tecnológicamente, se implementará la solución utilizando React (Next.js) y Tailwind CSS para asegurar un desarrollo ágil y una experiencia de usuario (UI/UX) fluida,
simulando las reglas de negocio del backend. El éxito de esta implementación se medirá a través de la reducción del tiempo de ciclo por solicitud (Time-to-Decision),
el incremento en el volumen de créditos procesados automáticamente sin intervención de los ejecutivos, y la tasa de conversión de usuarios durante el onboarding.

---

## Desglose de la Definición

* **¿Cuál es el problema a resolver?**
  El flujo actual requiere que el equipo de colaboradores contacte manualmente a cada prospecto para recopilar datos, verificar identidad y evaluar la viabilidad del crédito.
  Este proceso uno a uno es lento, propenso a errores y no es escalable ante un aumento drástico de la demanda, limitando el crecimiento de la empresa por falta de capacidad operativa.

* **¿Cómo lo quieres resolver?**
  Trasladando el esfuerzo de carga de datos al usuario final mediante un flujo de *onboarding* digital.
  El sistema guiará al cliente por un formulario por pasos, evaluará automáticamente los datos mediante un motor de reglas (scoring simulado) y, si el prospecto califica,
  emitirá un contrato digital para su aceptación inmediata. Los colaboradores solo intervendrán en casos de excepción o soporte.

* **¿Qué tecnologías quieres usar?**
  * **Frontend:** React (Next.js)
  * **Estilos y UI:** Tailwind CSS
  * **Gestión de Estado:** React Context
  * **Mock Backend:** Rutas de API de Next.js que devuelvan respuestas estáticas para simular la aprobación/rechazo y la generación del contrato.

* **¿Cómo vas a medir el éxito de tu implementación?**
  1. **Reducción del Tiempo de Operación:** Disminución del tiempo promedio desde que el usuario muestra interés hasta la firma del contrato (de horas/días a minutos).
  2. **Tasa de Automatización (Straight-Through Processing):** Porcentaje de solicitudes que se completan de inicio a fin sin ninguna intervención manual del equipo.
  3. **Tasa de Conversión y Abandono (Drop-off rate):** Monitoreo de en qué paso del formulario los usuarios abandonan el proceso, lo que permitirá iterar y mejorar la fricción en la UX.

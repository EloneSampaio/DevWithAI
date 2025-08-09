# PROMPT TEMPLATE PARA DOCUMENTAÇÃO DE PROJETOS

## Instrução Principal para IA

```
Crea una documentación completa y profesional para mi proyecto siguiendo esta estructura detallada. Adapta el contenido según el tipo de proyecto, pero mantén siempre la organización y nivel de detalle mostrado en el ejemplo.

INFORMACIÓN DEL PROYECTO:
- Nombre del proyecto: [INSERTAR_NOMBRE]
- Cliente/Empresa: [INSERTAR_CLIENTE]
- Tipo de proyecto: [INSERTAR_TIPO] (ej: desarrollo web, sistema ERP, app móvil, migración de datos, etc.)
- Tecnologías principales: [INSERTAR_TECNOLOGÍAS]
- Fecha de inicio: [INSERTAR_FECHA_INICIO]
- Fecha de entrega: [INSERTAR_FECHA_ENTREGA]
- Equipo disponible: [INSERTAR_EQUIPO] (ej: 1 desarrollador, 2 desarrolladores + 1 diseñador, etc.)
- Contexto adicional: [INSERTAR_CONTEXTO_ESPECÍFICO]

ESTRUCTURA REQUERIDA:

1. **TÍTULO Y DESCRIPCIÓN**
   - Título profesional con nombre del proyecto y cliente
   - Descripción detallada del proyecto y sus objetivos
   - Sección de tecnologías base utilizadas

2. **OBJETIVOS DEL PROYECTO**
   - Lista de 5-7 objetivos específicos y medibles
   - Cada objetivo debe estar en negrita y ser claro

3. **FLUJO DE IMPLEMENTACIÓN DETALLADO**
   - Dividir el proyecto en fases lógicas (mínimo 8, máximo 20 fases)
   - Para cada fase incluir:
     * **Objetivo**: Qué se busca lograr
     * Lista detallada de actividades específicas
     * Entregables esperados

4. **CRONOGRAMA ESTIMADO**
   - Tabla con fechas específicas calculadas según el tiempo disponible
   - Si el tiempo es muy ajustado, crear cronograma acelerado con advertencias
   - Incluir hitos críticos
   - Especificar duración total

5. **ENTREGABLES DEL PROYECTO**
   - Lista completa de lo que se entregará al final
   - Documentación técnica y de usuario
   - Código, sistemas, etc.

6. **BENEFICIOS ESPERADOS**
   - Lista de beneficios cuantificables cuando sea posible
   - Impacto en el negocio/organización

7. **REQUISITOS Y CONSIDERACIONES** (si aplica)
   - Pre-requisitos técnicos
   - Limitaciones identificadas
   - Recomendaciones para el éxito del proyecto

INSTRUCCIONES ESPECÍFICAS:
- Usa terminología técnica apropiada para el tipo de proyecto
- Mantén un tono profesional y detallado
- Calcula fechas realistas basadas en el tiempo disponible
- Si el cronograma es muy ajustado, incluye advertencias y estrategias de mitigación
- Adapta las fases según el tipo de proyecto (desarrollo, implementación, migración, etc.)
- Incluye tablas markdown bien formateadas
- Usa emojis de advertencia (⚠️) para puntos críticos
- Incluye checkboxes (✅) para requisitos o pre-condiciones

EJEMPLO DE ADAPTACIÓN POR TIPO DE PROYECTO:
- **Desarrollo Web**: Fases de diseño, frontend, backend, testing, deploy
- **App Móvil**: Fases de wireframes, UI/UX, desarrollo iOS/Android, testing, publicación
- **Sistema ERP**: Fases de análisis, configuración, migración datos, capacitación, go-live
- **E-commerce**: Fases de setup, catálogo, pagos, shipping, testing, lanzamiento

Genera el README.md completo siguiendo exactamente esta estructura y nivel de detalle.
```

## Ejemplo de Uso

Para usar este prompt, simplemente:

1. **Copia el prompt completo de arriba**
2. **Rellena la información específica de tu proyecto:**
   ```
   - Nombre del proyecto: Sistema de Ventas Online para Boutique Fashion
   - Cliente/Empresa: Boutique Fashion Madrid
   - Tipo de proyecto: E-commerce con gestión de inventario
   - Tecnologías principales: React, Node.js, MongoDB, Stripe
   - Fecha de inicio: 15 de enero de 2025
   - Fecha de entrega: 28 de febrero de 2025
   - Equipo disponible: 2 desarrolladores fullstack + 1 diseñador UX
   - Contexto adicional: Boutique física que quiere expandir online, 500 productos iniciales
   ```

3. **Envía a tu IA favorita (ChatGPT, Claude, etc.)**

## Variaciones del Prompt por Tipo de Proyecto

### Para Proyectos de Desarrollo Web/App:
Añadir: "Incluye fases específicas de: análisis de requisitos, diseño UX/UI, desarrollo frontend, desarrollo backend, integración de APIs, testing, despliegue y mantenimiento."

### Para Proyectos de Migración/Implementación:
Añadir: "Incluye fases específicas de: análisis del sistema actual, planificación de migración, backup de datos, migración por fases, testing paralelo, capacitación de usuarios y go-live."

### Para Proyectos de Consultoría:
Añadir: "Incluye fases específicas de: diagnóstico inicial, análisis detallado, propuesta de soluciones, implementación de mejoras, medición de resultados y entrega de documentación."

## Tips para Mejores Resultados

1. **Sé específico** en el contexto del proyecto
2. **Incluye restricciones** conocidas (presupuesto, tiempo, recursos)
3. **Menciona stakeholders** importantes
4. **Especifica el nivel técnico** del cliente (técnico vs no técnico)
5. **Indica si hay sistemas existentes** que integrar

Este template te generará documentación profesional y detallada para cualquier tipo de proyecto que inicies.
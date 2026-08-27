# Producto y arquitectura a futuro

## Principio: portal, productos y núcleo

La plataforma tendrá tres niveles distintos.

| Nivel | Responsabilidad | Ejemplos |
| --- | --- | --- |
| Portal principal | Marca, marketing, documentación, aprendizaje, catálogo, descargas y SEO. | Página institucional, casos de uso, guía de normas. |
| Productos especializados | Resolver una tarea específica con interfaz y flujo propios. | Predimensionamiento estructural, auditor de planillas, inspección de fisuras. |
| Núcleo compartido | Reglas técnicas y servicios reutilizables cuando estén maduros. | Unidades, formatos de informe, versionado de normas, archivos de proyecto. |

No se debe crear el núcleo compartido de forma abstracta. Solo se extraerá aquello que dos o más productos realmente necesiten.

## Aplicaciones web y de escritorio

La web es el mejor canal para encontrar la marca, enseñar, probar herramientas ligeras y publicar contenido. Las aplicaciones de escritorio son adecuadas cuando se necesite trabajo offline, archivos locales, alto rendimiento, proyectos grandes, privacidad o integración con el sistema del usuario.

La arquitectura será híbrida, no una elección excluyente:

```text
Portal web → descubre, aprende, descarga
Herramienta web → calcula o prueba tareas ligeras
Aplicación escritorio → trabaja en proyectos y archivos locales
Servicios opcionales → respaldo, sincronización, actualización, colaboración
```

La ausencia inicial de base de datos no bloquea el producto. Los primeros proyectos pueden guardarse como archivos locales. Una nube o cuentas se agregan solo cuando resuelvan una necesidad real.

## Archivos de proyecto

En el futuro se diseñará un formato propio de proyecto. El nombre y extensión dependen de la nueva marca; por ahora se denomina `proyecto.[extensión-pendiente]`.

El archivo debe poder contener, según el producto:

- Metadatos del proyecto.
- Norma, edición y versión del motor de cálculo.
- Unidades y materiales.
- Entradas, resultados y advertencias.
- Elementos estructurales o inspecciones.
- Historial de cambios relevante.
- Referencias usadas para los informes.
- Archivos adjuntos cuando aplique.

Se prefiere un formato portable, versionable y legible mediante herramientas técnicas; inicialmente podría ser un paquete con datos estructurados. La forma exacta se decidirá al crear la primera aplicación de escritorio.

## Motor de ingeniería

Todo cálculo profesional debe seguir estas reglas:

1. Separarse de la interfaz gráfica.
2. Tener pruebas automatizadas con ejemplos conocidos.
3. Declarar norma, versión, supuestos y limitaciones.
4. Validar unidades y rangos de entrada.
5. Exponer resultados intermedios importantes.
6. Generar resultados repetibles para las mismas entradas.
7. Evitar resultados ambiguos: una advertencia debe ser clara y accionable.

## IA: alcance permitido

La IA puede:

- Explicar resultados y ecuaciones ya calculadas.
- Detectar inconsistencias de entrada o de unidades.
- Ayudar a encontrar información dentro del proyecto.
- Proponer listas de revisión.
- Redactar borradores de memoria, siempre identificables y revisables.

La IA no puede:

- Ser la fuente de una ecuación normativa.
- Cambiar entradas o resultados sin confirmación y registro.
- Emitir un dictamen profesional autónomo.
- Ocultar incertidumbre, supuestos o falta de información.

## Tecnología

La tecnología no está decidida. Se escogerá por requisitos reales al iniciar cada producto.

- El portal puede priorizar rendimiento, SEO y contenido estático; Astro es un candidato fuerte.
- Las herramientas web pueden evolucionar desde la base React/TypeScript existente si conviene.
- Para escritorio se evaluarán Java/JavaFX, Tauri, Electron u otras alternativas frente a criterios como rendimiento, tamaño, reutilización de código, manejo de archivos, gráficos, soporte multiplataforma y curva de aprendizaje.

No se elegirá ahora un lenguaje que obligue a todos los productos futuros. La decisión que sí es permanente es separar el dominio de ingeniería de la interfaz.

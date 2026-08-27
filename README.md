# Plataforma ecuatoriana de herramientas de ingeniería civil

> Documento maestro de contexto. Léelo completo antes de proponer cambios de marca, producto, arquitectura o estrategia.

## Estado del proyecto

Esta carpeta define la reestructuración de una familia de proyectos de ingeniería civil creada por **Axel Hernández**, estudiante de Ingeniería de Software e ingeniero civil titulado, vinculado a la PUCE sede Portoviejo.

La iniciativa nace de una observación concreta: en ingeniería civil, muchos cálculos rutinarios siguen resolviéndose en Excel, mientras que el software profesional suele ser costoso, complejo y sobredimensionado para tareas puntuales. Existe una oportunidad para crear herramientas verificables, claras y accesibles, inicialmente orientadas a Ecuador y a la NEC.

El proyecto anterior más avanzado se llamaba **CivilKit EC / PreDim NEC**. Ese nombre se reemplazará: la marca final todavía no está decidida. Ecuador se mantiene expresamente como parte de la identidad y del propósito de posicionamiento mundial.

## Visión

Crear un ecosistema ecuatoriano de herramientas digitales de ingeniería civil que permita trabajar con proyectos, cálculos verificables, normas versionadas, informes claros y asistencia de IA, sin sustituir el criterio ni la responsabilidad del ingeniero.

No se busca copiar Autodesk por tamaño ni intentar hacer un único programa gigante. Se busca construir, gradualmente, una familia de productos especializados, conectados por una marca, estándares de calidad y formatos de proyecto compatibles.

## Principio rector

```text
Datos del usuario → motor normativo determinista → verificaciones → resultados trazables → informe
                                        ↑
                            IA para explicar, detectar y asistir
```

La IA no debe inventar ecuaciones, alterar resultados en silencio ni reemplazar el análisis profesional. El motor de cálculo, sus entradas, ecuaciones, referencias y versión deben ser auditables.

## Decisiones ya tomadas

- La marca anterior CivilKit dejará de ser el nombre final; se definirá una nueva marca.
- Ecuador no se eliminará de la identidad. El objetivo es llevar una propuesta ecuatoriana a reconocimiento internacional.
- Existirá un portal web principal, profesional y enfocado en marketing, documentación, descubrimiento y descargas.
- Cada herramienta tendrá una interfaz y flujo especializado. No se volverá a concentrar todo en una sola pantalla o producto monolítico.
- Se construirá una herramienta a la vez; no se iniciará el producto siguiente hasta que el actual pase su definición de terminado.
- Las herramientas podrán convivir y conectarse de forma gradual, pero no se forzará una integración temprana.
- En el futuro habrá aplicaciones de escritorio con trabajo offline y archivos de proyecto propios. La tecnología se decidirá por necesidad de cada producto, no por preferencia anticipada.
- El primer frente de trabajo es el portal principal y la identidad; el primer producto estructurado se definirá y se llevará a un estándar de lanzamiento antes de continuar.
- Todas las experiencias de producto incluirán un huevo de pascua sobrio: **“Axel was here”**.

## Proyectos existentes y su lugar

| Proyecto previo | Situación | Posible lugar futuro |
| --- | --- | --- |
| PreDim NEC / CivilKit EC | El más maduro; incluye módulos de cargas, tributarias, vigas, columnas, losas, deflexión y zapatas preliminares. | Candidato para convertirse en el primer producto estructural de la nueva marca. |
| PlanillaCheck | Prototipo de auditoría de planillas. | Producto futuro independiente para revisar y documentar hojas de cálculo de ingeniería. |
| CrackExpert AI | Proyecto de visión artificial y sistema experto para fisuras en hormigón. | Producto futuro de inspección; requiere maduración y validación separada. |

## Estructura deseada del ecosistema

```text
[Nueva marca Ecuador]
├── Portal principal
│   ├── catálogo de productos
│   ├── documentación y aprendizaje
│   ├── descargas
│   ├── normas y metodología
│   └── presencia de marca / contacto
├── Producto 01: estructural (por definir nombre final)
├── Producto 02: auditoría de planillas
├── Producto 03: inspección de fisuras
└── Servicios compartidos, solo cuando hagan falta
    ├── identidad visual y diseño
    ├── reportes
    ├── actualizaciones
    ├── sincronización opcional
    └── formato de proyecto
```

## Orden de trabajo actual

1. Definir nombre, identidad y narrativa de marca.
2. Diseñar y publicar el portal principal.
3. Elegir y delimitar el primer producto bajo la nueva marca.
4. Reconstruir o migrar ese producto con calidad de lanzamiento.
5. Lanzarlo, documentarlo y sostener marketing de contenido.
6. Solo entonces iniciar el siguiente producto.

Las fases detalladas están en [03-roadmap-y-fases.md](03-roadmap-y-fases.md). La guía para continuar con otra IA está en [06-contexto-para-ia.md](06-contexto-para-ia.md).

## Regla de calidad

“Terminado” no significa perfecto ni libre de mejoras. Significa que el producto cumple una lista explícita de requisitos técnicos, de validación, experiencia, documentación y lanzamiento. Cada producto tendrá su propio documento de aceptación.

## Próxima decisión humana

Definir el nombre de marca. No se debe elegir dominio, extensión de archivo, logo final ni nombres de productos hasta que exista una propuesta de nombre con verificación de disponibilidad, pronunciación y coherencia.

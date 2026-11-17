# Tarea: Mi prompt avanzado

## Tarea elegida

Diseñar un sistema de inventario para una tienda pequeña utilizando Java. El sistema permitirá registrar productos, consultar el inventario y actualizar el stock.

## Versión 1: prompt básico

CREA UN SISTEMA DE INVENTARIO PARA UNA TIENDA EN JAVA.

**Técnica agregada:** Ninguna. Es un prompt básico.

**¿Por qué?** Quería observar qué respuesta genera la IA con una instrucción sencilla.

**¿Qué mejoró en la respuesta?** La IA propuso una solución inicial, pero podía ser muy general y no especificar claramente los requisitos, las clases ni las validaciones necesarias.

## Versión 2: prompt con rol y contexto

```text
Actúa como desarrollador Java que diseña aplicaciones
para pequeñas tiendas.

Necesito un sistema de inventario que permita registrar
productos, mostrar el inventario, buscar productos por
código y actualizar el stock.

Utiliza Java y explica la función de cada clase.
```

**Técnicas agregadas:** Role prompting y contexto.

**¿Por qué?** El rol define el perfil desde el cual responde la IA y el contexto explica qué necesita el sistema.

**¿Qué mejoró en la respuesta?** La propuesta se volvió más específica e incluyó las funciones principales del inventario y una explicación de las clases.

## Versión 3: prompt final avanzado

```text
<rol>
Actúa como desarrollador Java especializado en aplicaciones
de consola para pequeñas tiendas.
</rol>

<contexto>
Estoy desarrollando un sistema de inventario como parte de
mi formación en Diseño y Desarrollo de Software.
El sistema debe ser sencillo, comprensible y funcional.
</contexto>

<tarea>
Desarrolla la solución siguiendo estos pasos:
1. Identifica los requisitos principales.
2. Diseña las clases y sus atributos.
3. Escribe el código Java completo.
4. Revisa la solución y propone mejoras.
</tarea>

<requisitos>
El sistema debe permitir:
- Registrar productos con código, nombre, precio y stock.
- Mostrar todos los productos registrados.
- Buscar productos por código.
- Actualizar la cantidad disponible.
- Evitar códigos duplicados y valores negativos.
</requisitos>

<ejemplo>
Producto: código 101, nombre Cuaderno, precio 5.50,
stock 20.
Resultado esperado al consultar:
Código: 101 | Nombre: Cuaderno | Precio: S/ 5.50 | Stock: 20
</ejemplo>

<formato>
Presenta los requisitos en una lista, las clases con sus
atributos y el código en bloques separados.
Utiliza Java y explica brevemente cómo ejecutar el programa.
</formato>

<autocritica>
Antes de finalizar, verifica que el código cumpla los
requisitos, que los nombres de las clases sean correctos,
que no existan códigos duplicados y que las validaciones
funcionen. Indica cualquier limitación que permanezca.
</autocritica>
```

**Técnicas agregadas:** Role prompting, descomposición, prompt estructurado, few-shot y autocrítica.

**¿Por qué?** Estas técnicas permiten definir el perfil de la IA, dividir el trabajo en pasos, organizar las instrucciones, mostrar un ejemplo del resultado esperado y revisar posibles errores.

**¿Qué mejoró en la respuesta?** La solución queda mejor organizada, los requisitos son más claros y resulta más sencillo comprobar si el código cumple con lo solicitado.

## Técnicas usadas en el prompt final

| Técnica | Parte del prompt | Función |
|---|---|---|
| Role prompting | `<rol>` | Define el perfil del desarrollador Java. |
| Descomposición | `<tarea>` | Divide el desarrollo en cuatro pasos. |
| Prompt estructurado | Etiquetas como `<contexto>` y `<formato>` | Organiza las instrucciones. |
| Few-shot | `<ejemplo>` | Muestra cómo debe verse un producto consultado. |
| Autocrítica | `<autocritica>` | Solicita revisar requisitos, código y validaciones. |

## Evaluación del resultado

| Criterio | Cumple (Sí/No) |
|---|---|
| El sistema permite registrar productos. | Sí |
| Permite buscar y mostrar productos. | Sí |
| Permite actualizar el stock. | Sí |
| Evita códigos duplicados y valores negativos. | Sí |
| El código está organizado y utiliza Java. | Sí |
| La IA identifica sus limitaciones. | Sí |

*Nota: estos criterios deben marcarse según la respuesta real de la IA y las pruebas realizadas al código.*

## Por qué elegí estas técnicas

Elegí estas técnicas porque permiten obtener una solución más clara y ordenada para un problema de programación. El rol establece el perfil de la IA, la descomposición ayuda a desarrollar el sistema por etapas y el prompt estructurado separa los requisitos. El ejemplo permite definir el formato esperado y la autocrítica ayuda a identificar posibles errores. No utilicé únicamente un prompt básico para no producir una solución incompleta o poco organizada.
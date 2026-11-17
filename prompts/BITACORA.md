# Bitacora de tecnicas avanzadas

Laboratorio 07: Tecnicas Avanzadas de Prompting.
Herramienta de IA usada: (escribe aqui cual usaste)

## Ejercicio 2: Zero-shot, one-shot y few-shot

 | Tipo | Aciertos (de 5) | Formato de la respuesta | Todas con el mismo formato (Si/No) |
|------|-----------------|-------------------------|------------------------------------|
| Zero-shot | No | desigual | Si, pero no era el formato |
| One-shot | Si | estructurado | Si |
| Few-shot | Si | estructurado | Si |


## Ejercicio 3: Chain of Thought

| Pedido | Respuesta de la IA | Muestra los pasos (Si/No) | Correcta (Si/No) |
|--------|--------------------|---------------------------|------------------|
| Directo | correcto | No | Si |
| Paso a paso | correcto | Si | Si |


## Ejercicio 4: Role prompting

| Version | Vocabulario (sencillo/tecnico) | Usa ejemplos o codigo | A quien le sirve mas |
|---------|-------------------------------|-----------------------|----------------------|
| A. Sin rol | sencillo | si | aprendices |
| B. Rol docente | sencillo | si | estudiantes |
| C. Rol senior | tecnico | si | personal tecnico |


## Ejercicio 5: Descomposicion

-Voy a crear un sistema de inventario para una tienda pequena en Java. Lista los 5 requisitos principales del sistema.

-Con esos requisitos, disena las clases necesarias. Para cada clase indica sus atributos con su tipo de dato.

-Escribe el codigo Java de la clase Producto con sus atributos, un constructor y los metodos get y set.

-Revisa el codigo de la clase Producto y propone 3 mejoras concretas.

## Ejercicio 6: Prompt estructurado y autocritica
```text
<rol>Actua como analista de pruebas de software.</rol>
<contexto>Login web con correo y contrasena. La cuenta se bloquea
despues de 3 intentos fallidos.</contexto>
<tarea>Piensa paso a paso que puede fallar y escribe 6 casos de prueba.</tarea>
<formato>Tabla con las columnas: ID, escenario, datos de entrada,
resultado esperado.</formato>

Revisa tu tabla: faltan casos limite como campos vacios, correo sin @
o contrasena con espacios? Agrega los que falten e indica cuales agregaste.
```

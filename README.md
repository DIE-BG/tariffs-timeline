# Cronología de aranceles

Línea de tiempo interactiva que documenta la evolución de las medidas comerciales y arancelarias de Estados Unidos. La visualización muestra las entradas en orden cronológico inverso (más reciente primero) con un diseño de columnas alternas para pantallas medianas y grandes.

## Archivos

| Archivo | Descripción |
|---|---|
| `index.html` | Página principal. Contiene todo el HTML, los estilos y la lógica de renderizado. |
| `data.js` | Datos de la cronología. Exporta el arreglo `newsData` que consume `index.html`. |

## Cómo agregar una nueva entrada

Abra `data.js` y agregue un objeto al arreglo `newsData`. El orden dentro del arreglo no importa visualmente (la página siempre muestra las entradas en orden cronológico inverso), pero por convención las entradas se agrupan en bloques `// FILA N` para mantener el archivo organizado.

### Estructura de un objeto

```js
{
    fecha:   "DD de mes YYYY",   // Texto libre; se muestra tal cual en la tarjeta
    resumen: "Descripción …",    // Texto del cuerpo de la tarjeta (ver formatos abajo)
    status:  "implemented",      // Ver valores permitidos más abajo
    fila:    1                   // Número de bloque; solo organizativo
}
```

### Valores de `status`

| Valor | Comportamiento |
|---|---|
| `"implemented"` | Entrada estándar, sin insignia adicional. |
| `"announced"` | Entrada estándar, sin insignia adicional. |
| `"threat"` | Muestra la insignia roja **Amenaza** en la tarjeta. |
| `"legal_ruling"` | Entrada estándar, sin insignia adicional. |

### Formato del campo `resumen`

El campo acepta texto plano. Se soportan los siguientes formatos especiales:

#### Saltos de línea

Use `\n` para insertar un salto de línea dentro del texto:

```js
resumen: "Primera línea.\n\nSegunda línea separada por párrafo."
```

Alternativamente, use una **plantilla literal** (backticks `` ` ``) para escribir el texto en varias líneas directamente en el archivo, sin necesidad de `\n`:

```js
resumen: `Primera línea.

Segunda línea separada por párrafo.`
```

Las líneas en blanco dentro de la plantilla literal se convierten en saltos de párrafo en la tarjeta, igual que `\n\n`. Los enlaces y demás formatos funcionan de la misma manera.

#### Hipervínculos

Use la sintaxis Markdown `[texto](url)` para insertar enlaces. La URL debe comenzar con `http://` o `https://`.

```js
resumen: "Descripción del evento. [Ver decreto](https://example.com/decreto)"
```

Se pueden incluir varios enlaces en la misma entrada:

```js
resumen: "Descripción del evento. [Fuente 1](https://example.com/1) y [Fuente 2](https://example.com/2)"
```

Los enlaces se abren en una pestaña nueva (`target="_blank"`).

### Ejemplo completo

Con `\n`:

```js
{
    fecha:   "21 de julio de 2026",
    resumen: "EE. UU. impone arancel del 50 % a una amplia gama de productos canadienses.\n\nSe salvan energía, potasa y minerales críticos. [Ver decreto](https://example.com/decree)",
    status:  "implemented",
    fila:    5
}
```

Con plantilla literal (equivalente):

```js
{
    fecha:   "21 de julio de 2026",
    resumen: `EE. UU. impone arancel del 50 % a una amplia gama de productos canadienses.

Se salvan energía, potasa y minerales críticos. [Ver decreto](https://example.com/decree)`,
    status:  "implemented",
    fila:    5
}
```

## Actualizar la versión del caché

`index.html` carga `data.js` con un parámetro de versión para evitar que los navegadores sirvan una copia desactualizada:

```html
<script src="data.js?v=20260609_v1"></script>
```

Cada vez que publique cambios en `data.js`, actualice ese parámetro con la nueva fecha (por ejemplo, `?v=20260721_v1`) para forzar la recarga en todos los navegadores.

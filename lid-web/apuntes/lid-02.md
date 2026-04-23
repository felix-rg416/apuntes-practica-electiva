# apuntes de la web del lid

Estuve buscando colores para la web del lid.

Le pregunté a algunas personas del lid qué color (además del negro) se les viene a la mente cuando piensan en el lid, la mayoría me dijo que el verde o colores neon.

Entonces busqué colores verdes en internet, lo puse en figma para ver colores y diagramación:

![verde y negro](.\imagenes\index-01-verde_negro.png)

![rosado y negro](.\imagenes\index-01-rosado_negro.png)

![celeste y negro](.\imagenes\index-01-celeste_negro.png)

![verde y negro](.\imagenes\index-02-verde_negro.png)

Empecé a poner los colores en el código CSS:

- Fondo: #000000
- Letras: #FFFFFF
- Enlaces: #39FF14
- Títulos: #39FF14

```css
:root {
  --background-color: #000000;
  --text-color: #FFFFFF;
  --text-color-heading: #39FF14;
  --text-color-link: #39FF14;
  --text-color-link-visited: #1DA600;
}
```

Primeros cambios:

![primeros cambios](.\imagenes\index-01.png)

## Siguiente paso: Diagramación

Ahora el plan es cambiar la diagramación de la página web.

Ponerle una barra de navegación más bonita y navegable para hacer que sea un página accesible y cómoda para todes

### pseudo código:

```css
. nav {
    ubicacion: inicio
    color: --nav-color
    color-texto: --text-nav-color
    ancho: 20%
    largo: 100%
    textos: alineados a la izquierda
}
```

en código sería:

```css
.nav {
    position: fixed;
    width: 20%;
    height: 100%;
    background-color: var(--nav-background-color);
    color: var(--text-nav-color);
    display: flex;
    flex-direction: column;
}
.nav a {
    color: var(--text-nav-color);
    text-decoration: none;
    padding: 10px;
    text-align: left;
}
```

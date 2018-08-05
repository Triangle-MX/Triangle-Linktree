# Triangle Linktree
Designed by: José Pablo Iglesias
Coded by: Mariano García

## Mockup
![Mockup](mockup.png)

[Mockup + Specs](https://xd.adobe.com/spec/3a3c9d16-8e8e-4308-5c75-ff861093c5ae-4c0d/)

## Especificaciones Importantes
### Emojis
Para que los emojis se vean en todas las plataformas usamos una librería llamada **Emoji CSS**. Encuentra la documentación [aquí](https://afeld.github.io/emoji-css/).

Para insertar un emoji se usa la siguiente estructura:
```html
<!-- Estructura Base -->
<i class="em-svg em-some-emoji"></i>

<!-- Ejemplos (Los tres Emojis que vas a usar) -->
<i class="em-svg em-male-technologist"></i>
<i class="em-svg em-male-artist"></i>
<i class="em-svg em-bulb"></i>
```

Usamos la clase `.em-svg` en vez de `.em` simplemente para que los emojis carguen como archivos `.svg` en vez de `.png`. Esto ahorra tiempo de carga.

### Colores y Otras Variables
#### Colores
- **Amarillo**: `#ffb61e`
- **Negro**: `#1b1b1b`
- **Blanco**: `#ffffff`

#### Transcisiones
- `transition: .3s ease-in-out`

#### Tipografías
- **Títulos y cosas importantes** (ósea todo en este caso): `font-family: 'Montserrat', 'Helvetica Neue', sans-serif;`
- **Texto General**: `font-family: 'Lato', 'Helvetica Neue', sans-serif;`

### Botones
CSS básico de los botónes (se le incluyen modificaciones en `main.css`):
```css
.btn-1 {
    display: inline-block;
    font-family: 'Montserrat', 'Helvetica Neue', sans-serif !important;
    padding: 8px 24px;
    background-color: #ffb61e;
    color: #ffffff !important;
    cursor: pointer !important;
    border-radius: 250px;
    font-size: 100% !important;
    font-weight: 400;
    -webkit-transition: .3s ease-in-out;
    -o-transition: .3s ease-in-out;
    transition: .3s ease-in-out;
}

.btn1:hover, .btn1:focus {
    -webkit-box-shadow: 0 0 30px 0 #ffb61e;
            box-shadow: 0 0 30px 0 #ffb61e;
    -webkit-transform: scale(1.05);
        -ms-transform: scale(1.05);
            transform: scale(1.05);
}

@media(max-width: 600px) {
    .btn-1 {
        padding: 5px 15px;
        font-size: 85% !important;
    }
}
```

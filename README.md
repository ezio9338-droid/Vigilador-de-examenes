# Vigilador de exámenes externos

Objetivo: vigilar exámenes que se hacen en otra plataforma (por ejemplo, Science Bits) con la misma vigilancia de salidas que el proyecto [Examenes_test](https://github.com/ezio9338-droid/Examenes_test).

Una página web no puede ver lo que pasa en otra pestaña. Por eso la idea es abrir el examen externo **dentro** de una página nuestra (en un marco) y vigilar esa página. Antes de construirlo hay que comprobar dos cosas en los dispositivos reales:

1. que la plataforma deja abrirse dentro de otra página, y
2. que dentro del marco se puede iniciar sesión (Safari en iPad bloquea por defecto las cookies de otras webs dentro de un marco).

## Página de prueba (`prueba.html`)

### Publicarla (una sola vez)

1. En este repositorio: **Settings → Pages**.
2. **Source: Deploy from a branch**, elige la rama donde esté `prueba.html` y la carpeta **`/ (root)`**. **Save**.
3. Al cabo de uno o dos minutos estará en `https://ezio9338-droid.github.io/Vigilador-de-examenes/prueba.html`.

### Hacer la prueba

En cada tipo de dispositivo (iPad del centro, ordenador del centro…):

1. Abre la página y pega el enlace de una tarea de Science Bits. **Cargar en el marco**.
2. Contesta en el apartado 2 lo que ves: si aparece Science Bits, si puedes iniciar sesión y si puedes contestar la tarea.
3. Toca dentro de la tarea y escribe algo: en «Señales» la salida debe seguir en **no**. Después cambia de app o de pestaña y vuelve: debe contarse.
4. En ordenadores, prueba también **Pantalla completa**.
5. **Copiar resultado** y pegarlo en la conversación.

La página no guarda ni envía nada. Del enlace solo muestra el dominio y la ruta, sin los parámetros.

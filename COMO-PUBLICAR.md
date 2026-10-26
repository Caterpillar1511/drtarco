# Cómo agregar videos y entradas al blog

Todo se puede hacer desde la página de GitHub, sin instalar nada. Después de guardar, la página se actualiza sola en uno o dos minutos.

## Agregar un video de YouTube

1. Abre el archivo `_data/videos.yml` y toca el lápiz (Edit).
2. Copia un bloque completo y pégalo al final, por ejemplo:

   ```yaml
   - titulo: Nombre del video
     youtube: CODIGO
     descripcion: Una frase sobre el video.
   ```

   El código es lo que va después de `v=` en el enlace de YouTube. En `https://www.youtube.com/watch?v=B_tTymvDWXk` el código es `B_tTymvDWXk`.
3. Respeta los espacios del inicio de cada línea y toca **Commit changes**.

## Escribir una entrada del blog

1. Entra a la carpeta `_posts` y toca **Add file → Create new file**.
2. Ponle de nombre la fecha y el título separados por guiones, terminado en `.md`, por ejemplo `2026-11-15-mi-primera-vuelta-en-bici.md`.
3. Copia esto al inicio y cambia los datos:

   ```
   ---
   layout: post
   title: Mi primera vuelta en bici por el llano
   tema: Ciclismo
   resumen: Una frase corta que se verá en la lista del blog.
   ---

   Aquí va el texto. Deja una línea en blanco entre párrafos.
   ```

4. Toca **Commit changes**. La entrada aparece de primera en la sección Blog.

Para poner una foto, súbela a la carpeta `assets` y agrega `imagen: /assets/nombre-de-la-foto.jpg` debajo de `resumen`.

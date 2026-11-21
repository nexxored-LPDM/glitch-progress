# Glitch Progress

Página pública de avances de Glitch Channel, preparada para GitHub Pages.

## Publicarla

1. Inicia sesión en GitHub y crea un repositorio nuevo llamado `glitch-progress`.
2. Deja el repositorio **público** si quieres que cualquiera pueda leer la página.
3. Sube `index.html` y `posts.json` a la raíz del repositorio.
4. En el repositorio, abre **Settings → Pages**.
5. En **Build and deployment**, elige **Deploy from a branch**.
6. Selecciona la rama `main` y la carpeta `/(root)`, y pulsa **Save**.
7. Espera a que termine la publicación. GitHub mostrará la dirección de la página en esa misma sección.

## Publicar un avance

1. Abre `posts.json` en el repositorio y pulsa el icono del lápiz para editarlo.
2. Añade un objeto al principio de la lista con este formato:

   ```json
   {
     "t": 1795218312692,
     "text": "Estamos preparando una nueva función para el canal."
   }
   ```

3. Cambia `t` por la fecha y hora en milisegundos desde la época Unix. En Linux Mint puedes obtener el valor actual en la terminal con:

   ```bash
   date +%s%3N
   ```

4. Conserva las comas entre objetos JSON, pulsa **Commit changes** y confirma el cambio.

GitHub Pages actualizará la página automáticamente. Para que solo tú puedas cambiar los avances, mantén el repositorio privado o, si el repositorio debe ser público, no añadas colaboradores con permiso de escritura. El HTML es público y de solo lectura: no contiene un formulario que pretenda guardar publicaciones sin autorización.

## Archivos

- `index.html`: página de lectura.
- `posts.json`: contenido del feed.

# PabloLopez2.github.io

## Página web de ejemplo de Lenguajes de Marcas (M04UF1)

Esta página es un test a modo de CV.

## Lista de tareas a hacer en la página

- [ ] Crear plantilla del cuerpo HTML

- [ ] Añadir navegación

- [ ] Crear etilo básico


### Ejercicio formularios revalidos

Para **validar** los formularios en HTML, podemos utilizar los atributos _required_ dentro de los campos del formulario.

Aquí dejo el código que he implemetado de los formularios, sé que el enunciado ponía 2 nuevos, pero me puse a investigar más y he descubierto un total de 8 nuevos formularios que son: radio, checkbox, number, file, range, search, tel y url.

```HTML
<p><label>Hobbies:</label>
		<p><label>Genero:</label>
        <input type="radio" name="gender" value="male"> Hombre
        <input type="radio" name="gender" value="female"> Mujer
        <input type="radio" name="gender" value="Non-binary"> No binario
        <input type="radio" name="gender" value="other"> Prefiero no decirlo</p>

	 	<p><label>Hobbies:</label>
        <input type="checkbox" name="hobby" value="reading"> Leer
        <input type="checkbox" name="hobby" value="traveling"> Viajar
        <input type="checkbox" name="hobby" value="photography"> Videojuegos</p>

        <p><label>Age:</label>
        <input type="number" name="age" min="18" max="100" required></p>

        <p><label>Upload file:</label>
        <input type="file" name="file"></p>

        <p><label>Rating:</label>
        <input type="range" name="rating" min="1" max="5" step="1" required></p>

        <p><label>Search:</label>
        <input type="search" name="search_term" required></p>

        <p><label>Phone number:</label>
        <input type="tel" name="phone_number" pattern="[0-9]{10}" required></p>

        <p><label>Website:</label>
        <input type="url" name="website" required></p>


        <p><input type="submit" value="Enviar" required/></p>
        </form> </main>
```

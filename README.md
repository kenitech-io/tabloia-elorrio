# ElorriON

Directorio de todas las actividades de Elorrio en un solo sitio: clases
particulares, academias, clubes deportivos, escuelas municipales, elkarteak y
lo que se hace en verano. Bilingüe (euskera / castellano), con contacto directo
con quien da la clase: sin pagos, sin comisiones y sin intermediarios.

**https://kenitech-io.github.io/tabloia-elorrio/**

El nombre se lee «Elorrion», que en euskera es «en Elorrio»: lo que hay en el
pueblo. El ON va en mayúsculas y se escribe así en todas partes. (El
repositorio y la URL todavía llevan el nombre anterior, `tabloia-elorrio`.)

---

## Esto es una demostración

Las fichas, las personas, los teléfonos, los precios y las valoraciones son
**inventados**: ninguna corresponde a una persona, un negocio ni una entidad
real de Elorrio. Las entidades públicas llevan «(adibidea)» en el nombre a
propósito. **Esta web no pertenece al Ayuntamiento de Elorrio ni está vinculada
a él**, y la revisión municipal que se describe es una propuesta, no un
servicio que exista hoy.

Las fotografías de las actividades son de archivo, con licencia libre (Flickr,
Wikimedia Commons, StockSnap). La autoría y la licencia de cada una están en
[`fotos/creditos.json`](fotos/creditos.json). La de la portada no: es una foto
del monte, aportada por el propietario de la web.

Mientras los datos sean inventados, la web lleva `noindex, nofollow`: quitarlo
es la primera casilla de la lista si algún día pasa a ser real.

## Cómo está hecho

Una web estática sin dependencias ni compilación:

```
index.html        todo: markup, estilos y lógica
fotos/            fotografías a 900×600
fotos/s/          las mismas a 560 px, para las tarjetas del móvil
fotos/t/          recortes cuadrados de 320 px, para las miniaturas de materia
fuentes/          Inter (fuente variable, 48 KB) servida desde aquí, no desde Google
```

Se abre con doble clic en `index.html` o se sirve con cualquier servidor
estático. No hay nada que instalar.

Las vistas tienen dirección propia, así que se pueden enlazar y compartir:

```
#/                          el buscador
#/?cat=idiomas&edad=7-11    con filtros puestos
#/ficha/18                  una actividad concreta
#/agenda                    las fechas del curso
#/guardados?ids=5,9,14      una lista para mandar por WhatsApp
#/publicar                  el formulario de alta
#/admin                     el panel de revisión (contraseña: demo)
```

## Si algún día se hace de verdad

Lo que hay aquí es la parte visible. Para que funcione hacen falta una base de
datos, altas reales y una persona que revise lo que llega. Dos reglas que
conviene no perder por el camino:

- **Nunca guardar el DNI ni el certificado de delitos sexuales.** Sólo
  «verificado por X el día Y». Los documentos se miran y no se almacenan.
- ElorriON no organiza las clases, no cobra comisión y no interviene en el
  pago. En cuanto lo haga, deja de ser esto.

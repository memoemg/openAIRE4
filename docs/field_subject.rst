.. _dci:subject:

Materia (MA)
============

``datacite:subject``

Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Materia, palabra clave, código de clasificación o frase clave que describe el recurso (ocurrencias: 0-n).


**Instrucciones de uso**

En la propiedad *subject* puede haber dos tipos de valores: ya sea una palabra clave o una clasificación.

En general, elija las palabras más significativas y únicas para las palabras clave y evite las que sean demasiado generales para describir un recurso en particular.

Para las palabras clave o frases clave que no estén controladas por un vocabulario o tesauro, separe con un punto y coma cada palabra clave o frase clave, o repita el elemento para cada término. No hay requisitos con respecto al uso de mayúsculas en las palabras clave, aunque se recomienda la consistencia interna (dentro de un mismo archivo).

En los casos en los que los términos se tomen de un esquema de clasificación estándar, codifique cada término mediante el uso de los atributos adicionales de la propiedad *subject*. Codifique todo el descriptor *subject* de acuerdo con el esquema relevante. Use las mayúsculas y la puntuación tal como están en el esquema original.

Se recomienda utilizar un URI cuando se usen esquemas de clasificación o vocabularios controlados, especialmente cuando se usen esquemas codificados como la Clasificación Decimal Dewey (DDC, por sus siglas en inglés) o la Clasificación Decimal Universal (UDC, por sus siglas en inglés). Los proveedores de servicios pueden reconocer esquemas de codificación más fácilmente cuando el esquema utiliza URIs en un espacio de nombres para la autoridad.

Si no se utiliza ningún esquema de clasificación específico, recomendamos usar la Clasificación Decimal de Dewey (DDC, por sus siglas en inglés). Se puede encontrar más información sobre la DDC y los Resúmenes de DDC en https://www.oclc.org/en/dewey/resources.html. Tenga en cuenta que OCLC posee todos los derechos de autor del Sistema de Clasificación Decimal de Dewey. Dewey, Dewey Decimal Classification, DDC, OCLC y WebDewey son marcas registradas de OCLC.

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad subject (MA, 0-n)
---------------------------

Utilice el nombre de la materia o la palabra clave como valor.

.. _dci:subject_subjectScheme:

Atributo subjectScheme (O)
--------------------------
Nombre del esquema de la materia o código de clasificación o autoridad, si se usa alguno de ellos (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Texto libre.

.. _dci:subject_schemeUri:

Atributo schemeURI (O)
----------------------
URI del esquema de identificador de materia (ocurrencia: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Ejemplos:

* http://id.loc.gov/authorities/subjects
* http://dewey.info/

Atributo valueURI (O)
---------------------
URI del término materia.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <datacite:subjects>
    <datacite:subject>Earth sciences and geology</datacite:subject>
    <datacite:subject subjectScheme="DDC" schemeURI="http://dewey.info/" valueURI="">
    551 Geology, hydrology, meteorology
    </datacite:subject>
   </datacite:subjects>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

.. _dc:publisher:

Editorial (MA)
==============

``dc:publisher``

Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Entidad responsable de hacer que el recurso esté disponible. Puede ser una persona, una organización o un servicio. Normalmente, el nombre de una editorial debe usarse para indicar la entidad.

**Instrucciones de uso**

Se trata de la editorial (ya sea comercial o no comercial) del recurso, no la (sub) institución de afiliación del autor. La editorial se usa solo en el sentido bibliográfico o funcional, no en el organizacional. Use solo el nombre completo de la editorial (comercial), no el nombre de cualquier organización o instituto que de otra manera [en un sentido más amplio] esté asociado con el creador.

Con las publicaciones universitarias, coloque el nombre de la facultad, el grupo de investigación o la escuela de investigación después del nombre de la universidad. En el caso de organizaciones donde claramente hay una jerarquía presente, incluya una lista de las partes de la jerarquía desde la más alta a la más baja, separadas por puntos. Si no está claro si hay una jerarquía presente o cuál es la parte más alta o más baja de la organización, indique el nombre tal como aparece en la impresión electrónica.

Es opcional usar nombres de editoriales tomados de listas de autoridades elaboradas a partir de listas de autoridades o tesauros locales o nacionales.

**No confundir con**

* :ref:`dci:contributor`
* :ref:`dci:creator`

En la mayoría de los casos, la editorial y el creador no son los mismos.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element publisher`_

Propiedad publisher (MA, 0-n)
-----------------------------

Utilice el nombre de la editorial como valor.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <dc:publisher>
     Loughborough University. Department of Computer Science
   </dc:publisher>
   <dc:publisher>John Wiley &amp; Sons, Inc. (US)</dc:publisher>

.. _DRIVER Guidelines v2 element publisher: https://wiki.surfnet.nl/display/DRIVERguidelines/Publisher

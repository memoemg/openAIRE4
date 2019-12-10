.. _dc:format:

Formato (R)
===========

``dc:format``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Manifestación física o digital del recurso. Normalmente, *Format* incluye el tipo de medio. *Format* puede usarse para determinar el software, el hardware u otro equipo necesario para mostrar u operar el recurso. Para tener una mejor práctica se recomienda seleccionar un valor de un vocabulario controlado (por ejemplo, la lista de Tipos de Medios de Internet [*MIME*, por sus siglas en inglés] que definen los formatos de medios de computadora)..

**Instrucciones de uso**

De acuerdo con las mejores prácticas, la lista registrada de IANA de los tipos de medios de Internet (tipos *MIME*) se utiliza para seleccionar un término. Para ver la lista completa, consulte http://www.iana.org/assignments/media-types

Si un recurso específico (una instancia de producción científica) tiene más de un formato físico (por ejemplo, postscript y pdf) almacenados como diferentes archivos de objetos, mencionar cada formato en una instancia del elemento Dublin Core (DC) ``format``, por ejemplo:

* ``<dc:format>application/pdf</dc:format>``
* ``<dc:format>application/postscript</dc:format>``
* ``<dc:format>application/vnd.oasis.opendocument.text</dc:format>``

**No confundir con**

* :ref:`aire:resourceType`
* :ref:`dci:identifier`
* :ref:`dci:size`

El elemento Dublin Core (DC) ``format`` describe el tipo de medio de este recurso. Por el contrario, ``oaire:resourceType``  describe el tipo de resultado académico que representa el recurso, mientras que ``datacite:identifier`` se utiliza para representar la manifestación del recurso digital.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element format`_

Propiedad format (R, 0-n)
-------------------------

Utilice el tipo de medio del recurso como valor.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <dc:format>video/quicktime</dc:format>
   <dc:format>application/pdf</dc:format>
   <dc:format>application/xml</dc:format>
   <dc:format>application/xhtml+xml</dc:format>
   <dc:format>application/html</dc:format>
   <dc:format>application/vnd.oasis.opendocument.text</dc:format>

.. _DRIVER Guidelines v2 element format: https://wiki.surfnet.nl/display/DRIVERguidelines/Format

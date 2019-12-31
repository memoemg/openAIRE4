.. _dc:source:

Fuente (R)
==========

``dc:source``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Referencia a un recurso del que se deriva el presente recurso.

**Instrucciones de uso**

El recurso actual puede derivarse del recurso ``source`` en su totalidad o en parte. Para tener una mejor práctica se recomienda referenciar el recurso por medio de una cadena o un número que se ajuste a un sistema de identificación formal.

Práctica recomendada: utilícese solo cuando el recurso descrito sea el resultado de la digitalización de originales no digitales. De lo contrario, use *:ref:`dci:relatedIdentifier`*. De forma opcional, se pueden agregar metadatos relacionados con la ubicación actual y el número de clasificación de la publicación digitalizada.

Use las directrices para la Codificación de Información Bibliográfica de Citas en los metadatos de Dublín Core (http://dublincore.org/documents/dc-citation-guidelines/).

**No confundir con**

* :ref:`dci:identifier`

**Observaciones**

* introducido en `DRIVER Guidelines v2 element source`_

Propiedad source (R, 0-n)
-------------------------

Use la información de la fuente como valor.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <dc:source>Ecology  Letters (1461023X)  vol.4 (2001)</dc:source>

.. _DRIVER Guidelines v2 element source: https://wiki.surfnet.nl/display/DRIVERguidelines/Source

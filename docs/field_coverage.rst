.. _dc:coverage:

Cobertura (R)
=============

``dc:coverage``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Alcance del contenido del recurso. La cobertura generalmente incluye un período temporal (una etiqueta de período, fecha o un rango de fechas).

**Instrucciones de uso**

Se recomienda utilizar valores literales o no literales. De ser necesario, repita este elemento para codificar múltiples períodos.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element coverage`_.
* para describir información de ubicación espacial (un nombre de lugar o coordenadas geográficas) use la propiedad :ref:`dci:geolocation`

Propiedad coverage (R, 0-n)
---------------------------

Utilice el período temporal como valor.

Ejemplo
~~~~~~~

Ejemplo temporal:

.. code-block:: xml
   :linenos:

   <dc:coverage>2000-2010</dc:coverage>

Ejemplo: nombre de un periodo:

.. code-block:: xml
   :linenos:

   <dc:coverage>
     scheme=historic; content=Ming Dynasty
   </dc:coverage>

.. _DRIVER Guidelines v2 element coverage: https://wiki.surfnet.nl/display/DRIVERguidelines/Coverage

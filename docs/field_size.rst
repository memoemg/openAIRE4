.. _dci:size:

Tamaño (O)
========

``datacite:size``

Cardinalidad
~~~~~~~~~~~~

*Opcional*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Información no estructurada sobre el tamaño del recurso.

**Valores permitidos, ejemplos y otras restricciones**

Texto libre.

Ejemplos: "15 páginas", "6 MB"

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad size (O, 0-n)
-----------------------

Use la información del tamaño como valor. Repita la propiedad para diferentes dominios de información de tamaño.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

     <datacite:sizes>
	     <datacite:size>15 pages</datacite:size>
	     <datacite:size>6 MB</datacite:size>
     </datacite:sizes>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

.. _dc:description:

Descripción (MA)
================

``dc:description``


Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Reseña del contenido del recurso. La descripción puede incluir entre otros elementos, un resumen, una tabla de contenido, una referencia a una representación gráfica del contenido o una reseña del contenido en texto libre.

**Instrucciones de uso**

Este elemento se utiliza para consignar una descripción textual del contenido. Cuando un recurso consta de varios archivos de objetos físicos por separado, no utilice ``dc:description`` para enumerar los URL de estos archivos.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element description`_

Propiedad description (MA, 0-n)
-------------------------------

Use la descripción textual como valor.

.. _dc:description_lang:

Atributo lang (O)
-----------------

Lenguaje de la descripción (ocurrencia: 0-1).

Use el atributo ``xml:lang`` para indicar el idioma de la descripción.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <dc:description>
     Foreword [by] Hazel Anderson; Introduction; The scientific heresy:
     transformation of a society; Consciousness as causal reality [etc]
   </dc:description>

   <dc:description xml:lang="en-US">
     A number of problems in quantum state and system identification are
     addressed.
   </dc:description>

.. _DRIVER Guidelines v2 element description: https://wiki.surfnet.nl/display/DRIVERguidelines/Description

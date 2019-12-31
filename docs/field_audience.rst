.. _dct:audience:

Audiencia (O)
=============

``dcterms:audience``

Cardinalidad
~~~~~~~~~~~~

*Opcional*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Clase de entidad a la que se destina o para la que es útil el recurso.

**Instrucciones de uso**

La clase de entidad puede determinarla el creador, la editorial o un tercero. Un ejemplo de audiencias se deriva del `Vocabulario de estándares comunes de datos de educación`_. Tenga en cuenta que esta no es una lista exhaustiva.

* Administradores
* Grupos de la comunidad
* Consejeros
* Receptores y solicitantes de fondos federales
* Bibliotecólogos
* Medios de comunicación
* Otros
* Padres y familias
* Autoridades que crean las políticas
* Investigadores
* Personal de apoyo escolar
* Proveedores de ayuda financiera para estudiantes
* Estudiantes
* Educadores

**Observaciones**

* introducido en `DRIVER Guidelines v2 element audience`_

Propiedad audience (O, 0-n)
---------------------------

Usa la clase de entidad como valor.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <dcterms:audience>Researchers</dcterms:audience>
   <dcterms:audience>Students</dcterms:audience>

.. _Common Education Data Standards vocabulary: https://ceds.ed.gov/element/001492
.. _DRIVER Guidelines v2 element audience: https://wiki.surfnet.nl/display/DRIVERguidelines/Audience

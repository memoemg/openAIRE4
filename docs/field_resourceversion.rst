.. _aire:version:

Versión del recurso (R)
=======================

``oaire:version``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Según el tipo de recurso, esta propiedad se utiliza para indicar:

* el número de versión de un conjunto de datos o software
* el estado del proceso de publicación de los artículos de una revista.

**Uso**

Para recursos de software y conjuntos de datos, se aceptará cualquier cadena; sin embargo, se recomienda una etiqueta con una versión semántica. Consulte <https://semver.org> para obtener más información sobre las versiones semánticas.

Para los artículos preliminares y los artículos finales que forman del proceso de publicación de una revista se debe usar un término controlado de las “Journal Article Versions (JAV): Recommendations of the NISO/ALPSP JAV Technical Working Group” (JAV). En castellano, "Versiones de Artículos de Revistas (JAV): Recomendaciones del Grupo de Trabajo Técnico NISO/ALPSP JAV" (`JAV`_). En este caso, la propiedad *debe* incluir el atributo ``uri``. El valor de la propiedad es la etiqueta correspondiente del URI HTTP.

Propiedad version (R, 1)
------------------------

Utilice un número de versión o la etiqueta del término de vocabulario como valor.

Atributo uri (MA)
-----------------

Los identificadores URI HTTP que se permiten están tomados del Vocabulario de tipos de versión COAR (`COAR Version Types Vocabulary`_).

**Version (controlled):**

=============================================== ========== =================================
URI del concepto                                Eiqueta    Comentario
=============================================== ========== =================================
http://purl.org/coar/version/c_b1a7d7d4d402bcce ``AO``     versión original del autor
http://purl.org/coar/version/c_71e4c1898caa6e32 ``SMUR``   versión sometida a revisión
http://purl.org/coar/version/c_ab4af688f83e57aa ``AM``     versión final del autor
http://purl.org/coar/version/c_fa2ee174bc00049f ``P``      prueba de galera
http://purl.org/coar/version/c_970fb48d4fbd8a85 ``VoR``    versión publicada
http://purl.org/coar/version/c_e19f295774971610 ``CVoR``   versión corregida
http://purl.org/coar/version/c_dc82b40f9837b551 ``EVoR``   versión mejorada
http://purl.org/coar/version/c_be7fb7dd8ff6fe43 ``NA``     versión desconocida
=============================================== ========== =================================

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <oaire:version>1.0.3</oaire:version>

.. code-block:: xml
   :linenos:

   <oaire:version uri="http://purl.org/coar/version/c_be7fb7dd8ff6fe43">AM</oaire:version>


.. _COAR Version Types Vocabulary: http://vocabularies.coar-repositories.org/documentation/version_types/
.. _JAV: https://www.niso.org/publications/niso-rp-8-2008-jav

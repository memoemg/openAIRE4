.. _aire:file:

Ubicación del archivo (MA)
==========================

``oaire:file``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Referencia no ambigua a los archivos con los que se asocia el recurso, por ejemplo, el texto completo. Repita la propiedad para cada archivo asociado.

Propiedad file (MA, 0-n)
------------------------

Utilice el URI HTTP del archivo como valor.

Atributo accessRightsURI (R)
----------------------------

Use los términos del Vocabulario de derechos de acceso de COAR (`COAR Access Right Vocabulary`_).

======================================== ========================
URI del concepto                               Etiqueta
======================================== ========================
http://purl.org/coar/access_right/c_abf2 ``acceso abierto``
http://purl.org/coar/access_right/c_f1cf ``acceso embargado``
http://purl.org/coar/access_right/c_16ec ``acceso restringido``
http://purl.org/coar/access_right/c_14cb ``registro bibliográfico``
======================================== ========================

Atributo mimeType (R)
---------------------

Especifique el formato de archivo. Se recomienda seleccionarlo a partir del tipo de medio MIME, el cual está registrado en IANA. Para ver la lista completa, consulte http://www.iana.org/assignments/media-types.

Atributo objectType (R)
-----------------------

Especifique el tipo de objeto que representa el archivo. Selecciónelo de la siguiente lista controlada:

* ``fulltext`` - texto completo
* ``dataset`` - conjunto de datos
* ``software`` - software
* ``other`` - otro

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <oaire:file accessRightsURI="http://purl.org/coar/access_right/c_abf2" mimeType="application/pdf" objectType="fulltext">http://link-to-the-fulltext.org</oaire:file>

.. _COAR Access Right Vocabulary: http://vocabularies.coar-repositories.org/documentation/access_rights/

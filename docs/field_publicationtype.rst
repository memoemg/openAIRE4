.. _aire:resourceType:

Tipo de recurso (M)
===================

``oaire:resourceType``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Tipo de producción científica de la que es manifestación el recurso. Describe el género del recurso.

**Uso**

El atributo ``resourceTypeGeneral`` se usa para categorizar el recurso como perteneciente a una clase principal de resultados de investigación.
El atributo ``uri`` contiene el URI HTTP del concepto de un tipo de recurso e indica la subpropiedad de ``resourceTypeGeneral``.
La etiqueta de este concepto se utiliza como valor para el elemento ``resourceType``.

**No confundir con**

* :ref:`dc:format` que describe el tipo de medio de este recurso.

**Observaciones**

* las versiones anteriores de las Directrices OpenAIRE utilizaban el `vocabulario info:eu-repo para tipos de publicaciones <https://wiki.surfnet.nl/display/standards/info-eu-repo/#info-eu-repo-Publicationtypes>`_.
* se adopta el elemento ``resourceType`` de DataCite MetadataKernel v4.1.
* se agrega a este perfil de aplicación el atributo ``uri`` para el URI del concepto de tipo de recurso.

Propiedad resourceType (M, 1)
-----------------------------

Utilice la etiqueta del término de tipo de recurso como valor. En la siguiente tabla se enumeran las etiquetas preferidas en inglés. Sin embargo, se pueden elegir etiquetas (preferidas o alternativas) en otros idiomas del Vocabulario de Tipos de Recursos de la Confederación de Repositorios de Acceso Abierto (COAR, por sus siglas en inglés).

Atributo resourceTypeGeneral (M)
--------------------------------

Se refiere al tipo general de un recurso.

*Valores de la lista controlada:*

* ``literature`` - literatura
* ``dataset`` - conjunto de datos
* ``software`` - software
* ``other research product`` - otro producto de investigación

Atributo uri (M)
----------------

Use términos del `Vocabulario de tipo de recurso de COAR (COAR Resource Type Vocabulary) <http://vocabularies.coar-repositories.org/documentation/resource_types/>`_ (ocurrencia: 1).

.. include:: vocabularies/resourcetype.rst

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <oaire:resourceType resourceTypeGeneral="literature" uri="http://purl.org/coar/resource_type/c_6501">journal article</oaire:resourceType>

.. _COAR Resource Type Vocabulary: http://vocabularies.coar-repositories.org/documentation/resource_types/

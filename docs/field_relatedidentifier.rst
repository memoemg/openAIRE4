.. _dci:relatedIdentifier:

Identificador relacionado (R)
=============================

``datacite:relatedIdentifier``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Identificador de un recurso relacionado distinto al identificador primario aplicado al recurso que se va a registrar.

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad relatedIdentifier (R, 0-n)
------------------------------------

Utilice el identificador relacionado como valor. Repita esta propiedad para cada identificador relacionado.

Atributo relatedIdentifierType (M)
----------------------------------

Tipo de identificador relacionado (ocurrencia: 1). Es obligatorio si se usa *relatedIdentifier*.

.. include:: vocabularies/relatedidentifiertype.rst

Atributo relationType (M)
-------------------------

Descripción de la relación entre el recurso que se va a registrar (A) y el recurso relacionado (B) (ocurrencia: 1). Es obligatorio si se usa *relatedIdentifier*.

.. include:: vocabularies/relationtype.rst

Atributo relatedMetadataScheme (O)
----------------------------------

Nombre del esquema (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Úsese solo con este par de relaciones: (``HasMetadata``/``IsMetadataFor``).


Atributo schemeURI (O)
----------------------

URI del esquema de metadatos relacionado señalado en *relatedMetadataScheme* (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Úsese solo con este par de relaciones: (``HasMetadata``/``IsMetadataFor``).


Atributo schemeType (O)
-----------------------

Se refiere al tipo de esquema de metadatos relacionado señalado en *relatedMetadataScheme*, vinculado con *schemeURI* (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Úsese solo con este par de relaciones: (``HasMetadata``/``IsMetadataFor``).

Ejemplos: ``XSD``, ``DDT``, ``Turtle``

Atributo resourceTypeGeneral (O)
--------------------------------

Se refiere al tipo general del recurso relacionado (ocurrencias: 0-1).

.. include:: vocabularies/resourcetypegeneral.rst

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:relatedIdentifiers>
      <datacite:relatedIdentifier relatedIdentifierType="URL" relationType="HasPart">http://someUrl</datacite:relatedIdentifier>
   </datacite:relatedIdentifiers>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

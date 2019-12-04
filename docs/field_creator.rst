.. _dci:creator:

Creador (M)
===========

``datacite:creator``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Ocurrencia: 1-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Autores de la publicación en orden de prioridad. Puede ser un nombre corporativo/institucional o personal.

**No confundir con**

* :ref:`dci:contributor`
* :ref:`dc:publisher`

**Remarks**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad creator (M, 1-n)
--------------------------


.. _dci:creator_creatorName:

Subpropiedad creatorName (M)
----------------------------

Nombre del autor (ocurrencia: 1). Consigunar con el formato: Apellido, Nombre. Los
nombres en alfabetos latinos pueden transliterarse siguiendo las normas de la `ALA-LC <http://www.loc.gov/catdir/cpso/roman.html>`_.

.. _dci:creator_nameType:

Atributo nameType (R)
*********************

Tipo de nombre (occurrence: 0-1).

.. include:: vocabularies/nametype.rst

.. _dci:creator_givenName:

Subpropiedad givenName (R)
--------------------------

Nombre propio o de pila del autor.

.. _dci:creator_familyName:

Subpropiedad familyName (R)
---------------------------

Apellido del autor.

.. _dci:creator_nameIdentifier:

Subpropiedad nameIdentifier (R)
-------------------------------

Identifica de forma única a una persona física o jurídica, según varios esquemas (ocurrencias: 0-n). El formato depende del esquema.

.. note::
   OpenAIRE recomienda incluir un identificador persistente de autor, tal como ORCID o ISNI cuando esté disponible.


.. _dci:creator_nameIdentifier_nameIdentifierScheme:

Atributo nameIdentifierScheme (M)
*********************************

Nombre del esquema de identificación de nombres (ocurrencia: 1). Es obligatorio si se usa la identificación de nombres [nameIdentifier].

.. _dci:creator_nameIdentifier_schemeURI:

Atributo schemeURI (R)
**********************

Identificador Uniforme de Recursos (URI) del esquema de identificación de nombres (ocurrencia: 0-1).

.. _dci:creator_affiliation:

Subpropiedad affiliation (R)
----------------------------

Afiliación organizacional o institucional del creador (ocurrencia: 0-n).

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <datacite:creators>
     <datacite:creator>
       <datacite:creatorName>Evans, R.J.</datacite:creatorName>
       <datacite:affiliation>Institute of Science and Technology</datacite:affiliation>
       <datacite:nameIdentifier nameIdentifierScheme="ORCID"
                       schemeURI="http://orcid.org">
         1234-1234-1234-1234
       </datacite:nameIdentifier>
     </datacite:creator>
   </datacite:creators>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
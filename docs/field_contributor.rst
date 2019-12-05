.. _dci:contributor:

Colaborador (MA)
=================

``datacite:contributor``

Cardinalidad
~~~~~~~~~~~~

*Es obligatorio si es aplicable*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Institución o persona responsable de recolectar, administrar, distribuir o contribuir de alguna otra manera al desarrollo del recurso.

**No confundir con**

* :ref:`dc:publisher`
* :ref:`dci:creator`
* :ref:`aire:fundingReference`

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad contributor (MA, 0-n)
-------------------------------


.. _dci:contributor_contributorType:

Atributo contributorType (M)
----------------------------

Tipo de colaborador del recurso (ocurrencia: 1). Es obligatorio si se utiliza *colaborador* [*contributor*].

.. include:: vocabularies/contributortype.rst

.. _dci:contributor_contributorName:

Subpropiedad contributorName (M)
--------------------------------

Nombre del colaborador (occurrence: 1). Es obligatorio si se utiliza colaborador [*contributor*].

.. _dci:contributor_nameType:

Atributo nameType (R)
*********************

Tipo de nombre (ocurrencia: 0-1).

.. include:: vocabularies/nametype.rst

.. _dci:contributor_familyName:

Subproiedad familyName (O)
--------------------------

Apellido del colaborador (ocurrencia: 0-1).

.. _dci:contributor_givenName:

Subpropiedad givenName (O)
--------------------------

Nombre propio o de pila del colaborador (ocurrencia: 0-1).


.. _dci:contributor_nameIdentifier:

Subpropiedad nameIdentifier (R)
-------------------------------

Identifica de forma única a una persona física o jurídica, según varios esquemas (ocurrencia: 0-n).

.. _dci:contributor_nameIdentifierScheme:

Atributo nameIdentifierScheme (M)
*********************************

Nombre del esquema de identificación de nombres (ocurrencia: 1). Es obligatorio si se usa *nameIdentifier*

.. _dci:contributor_schemeURI:

Atributo schemeURI (R)
**********************

URI del esquema de identificación de nombres (ocurrencia: 0-1).

.. _dci:contributor_affiliation:

Subpropiedad affiliation (R)
----------------------------

Afiliación organizacional o institucional del colaborador.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:contributors>
	   <datacite:contributor>
	     <datacite:contributorName>Evans, R. J.</datacite:contributorName>
	   <datacite:contributor>
	   <datacite:contributor>
	     <datacite:contributorName>International Human Genome Sequencing Consortium</datacite:contributorName>
	   </datacite:contributor>
   </datacite:contributors>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

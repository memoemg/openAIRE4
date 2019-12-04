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

Tipo de colaborador del recurso (ocurrencia: 1). Es obligatorio si se utiliza *colaborador* [contributor].

.. include:: vocabularies/contributortype.rst

.. _dci:contributor_contributorName:

Subpropiedad contributorName (M)
--------------------------------

Nombre del colaborador (occurrence: 1). Es obligatorio si se utiliza *colaborador* [contributor].

.. _dci:contributor_nameType:

Atributo nameType (R)
*********************

Tipo de nombre (ocurrencia: 0-1).

.. include:: vocabularies/nametype.rst

.. _dci:contributor_familyName:

Subproperty familyName (O)
--------------------------

The surname or last name of the contributor (occurrence: 0-1).

.. _dci:contributor_givenName:

Subproperty givenName (O)
-------------------------

The personal or first name of the contributor (occurrence: 0-1).


.. _dci:contributor_nameIdentifier:

Subproperty nameIdentifier (R)
------------------------------

Uniquely identifies an individual or legal entity, according to various schemes (occurrence: 0-n).

.. _dci:contributor_nameIdentifierScheme:

Attribute nameIdentifierScheme (M)
**********************************

The name of the name identifier scheme (occurrence: 1). Mandatory if *nameIdentifier* is used.

.. _dci:contributor_schemeURI:

Attribute schemeURI (R)
***********************

The URI of the name identifier scheme (occurrence: 0-1).

.. _dci:contributor_affiliation:

Subproperty affiliation (R)
---------------------------

The organisational or institutional affiliation of the contributor.

Example
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

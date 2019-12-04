.. _aire:fundingReference:

Referencia de financiamiento (MA)
=================================

``oaire:fundingReference``

Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda.*

*Ocurrencia: 0-n.*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Información sobre el apoyo financiero (financiamiento) para el recurso que se va a registrar.

**Instrucciones de uso**

.. include:: projectid.rst

**Observaciones**

* se introdujo como ``info:eu-repo/grantAgreement`` en versiones anteriores de las Directrices de OpenAIRE.
* se adopta el elemento fundingReference y sus subpropiedades de DataCite MetadataKernel v4.1, el cual reemplaza la sintaxis ``info:eu-repo/grantAgreement``.
* adding subproperty fundingStream to this application profile

Propiedad fundingReference (MA, 0-n)
------------------------------------

Repita esta propiedad para indicar los diferentes financiadores y proyectos.

Subpropiedad funderName (M)
---------------------------

Nombre del proveedor del financiamiento (ocurrencia: 1). Es obligatorio si se usa *fundingReference*.

Subpropiedad funderIdentifier (R)
---------------------------------

Identificador único de la entidad financiadora (ocurrencia: 0-1).

Atributo funderIdentifiertype (R)
*********************************

Type of the unique identifier of the funding entity (occurrence: 0-1).

.. include:: vocabularies/funderidentifiertype.rst

Véase también `Registro de Financiadores de Crossref (Crossref Funder Registry) <http://fundref.org/services/funder-registry>`_

Subpropiedad fundingStream (O)
------------------------------

Nombre de la vía de financiamiento (opcional) (ocurrencia: 0-1).

Subpropiedad awardNumber (MA)
-----------------------------

Project grantId or awardNumber (occurrence: 1).

Atributo awardURI (R)
*********************

URI de la página de presentación del proyecto proporcionada por el financiador para obtener más información sobre la adjudicación (subvención) (ocurrencia: 0-1). 

Subpropiedad awardTitle (R)
---------------------------

Título del proyecto, adjudicación o subvención (ocurrencia: 0-1).


Ejemplo
~~~~~~~

El siguiente es un ejemplo en el que se utilizan todos los campos:

.. code-block:: xml
   :linenos:

   <oaire:fundingReferences>
    <oaire:fundingReference>
     <oaire:funderName>European Commission</oaire:funderName>
     <oaire:funderIdentifier funderIdentifierType="Crossref Funder ID">http://doi.org/10.13039/100010661</oaire:funderIdentifier>
     <oaire:fundingStream>Horizon 2020 Framework Programme</oaire:fundingStream>
     <oaire:awardNumber awardURI="http://cordis.europa.eu/project/rcn/194062_en.html">643410</oaire:awardNumber>
     <oaire:awardTitle>Open Access Infrastructure for Research in Europe 2020</oaire:awardTitle>
    </oaire:fundingReference>
   </oaire:fundingReferences>

.. _Crossref Funder Registry: http://fundref.org/services/funder-registry

.. _dci:alternativeIdentifier:

Identificador alternativo (R)
=============================

``datacite:alternateIdentifier``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Cualquier otro identificador distinto al identificador primario aplicado al recurso que se va a registrar.  Puede ser cualquier cadena alfanumérica que sea única dentro de su dominio de emisión. Puede utilizarse para identificadores locales. AlternateIdentifier debe utilizarse para indicar otro identificador de la misma instancia (misma ubicación, mismo archivo).

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad alternateIdentifier (R, 0-n)
--------------------------------------

Valor del identificador alternativo.

Attribute alternateIdentifierType (M)
-------------------------------------

Tipo del identificador alternativo (ocurrencia: 1). Es obligatorio si se usa AlternateIdentifier.

Se *recomienda* tomar el valor de la siguiente lista:

.. include:: vocabularies/relatedidentifiertype.rst

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:alternateIdentifiers>
      <datacite:alternateIdentifier alternateIdentifierType="URL">http://someUrl</datacite:alternateIdentifier>
   </datacite:alternateIdentifiers>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

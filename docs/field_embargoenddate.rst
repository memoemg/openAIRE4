.. _dci:dateEmbargo:

Fecha del período de embargo (MA, 2)
=================================

``datacite:date``


Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda*

*Ocurrencia: 2*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Fechas relevantes para describir un período de embargo.

Representa la fecha en que se hace público el recurso disponible. Puede ser un rango. Para indicar la fecha de fin de un embargo, use el tipo de fecha ``Available`` en este elemento. La mejor práctica recomendada para codificar el valor de la fecha se define en un perfil de la norma ISO 8601 [W3CDTF] y sigue el formato ``AAA-MM-DD``.

**Observaciones**

* introducido como `info:eu-repo/date/embargoEnd/[YYYY-MM-DD] <https://wiki.surfnet.nl/display/standards/info-eu-repo/#info-eu-repo-DateTypesandvalue>`_ en versiones anteriores de las Directrices de OpenAIRE.
* esta versión del perfil de aplicación adopta el elemento date en combinación con atributos *dateType* de DataCite MetadataKernel v4.1, con lo cual se  reemplaza la sintaxis: ``info:eu-repo/date/EmbargoEnd``.

Cuando :ref:`dci:accessrights` toma el siguiente valor::

    <datacite:rights uri="http://purl.org/coar/access_right/c_f1cf">embargoed access</<datacite:rights>

se debe proporcionar la fecha de inicio y finalización del período de embargo.

Propiedad date (MA, 2)
----------------------

Use la fecha de inicio del embargo como valor en una instancia y la fecha de finalización en otra instancia.

Atributo dateType (M)
---------------------

Tipo de fecha. Elija del vocabulario de :ref:`tipo de fecha <vocab:datetype_datetype>` el término controlado ``Accepted`` para indicar el inicio y el término ``Available`` para indicar el final de un período de embargo.

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <datacite:dates>
     <datacite:date dateType="Accepted">2011-12-01</datacite:date>
     <datacite:date dateType="Available">2012-12-01</datacite:date>
   </datacite:dates>

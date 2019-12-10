.. _dci:accessrights:

Derechos de acceso (M)
======================

``datacite:rights``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Derechos de acceso del recurso.

Indica la información sobre los derechos o el modo en que se puede acceder el recurso. Si los metadatos describen más de un recurso, por ejemplo, un texto completo y el material complementario, se debe proporcionar la información sobre los derechos de acceso del recurso principal.

Use los términos del Vocabulario de derechos de acceso de COAR `(COAR Access Right Vocabulary) <http://vocabularies.coar-repositories.org/documentation/access_rights/>`_ (ocurrencia: 1).

======================================== ==========================
URI del concepto                               Etiqueta
======================================== ==========================
http://purl.org/coar/access_right/c_abf2 ``acceso abierto``
http://purl.org/coar/access_right/c_f1cf ``acceso embargado``
http://purl.org/coar/access_right/c_16ec ``acceso restringido``
http://purl.org/coar/access_right/c_14cb ``registro bibliográfico``
======================================== ==========================

.. note::
   A diferencia de DataCite, OpenAIRE restringe el uso de esta propiedad solo para indicar el derecho de acceso. 

**No confundir con**

* :ref:`aire:licenseCondition` (Use ``oaire:licenseCondition`` para obtener información sobre la licencia relacionada con el recurso).

**Observaciones**

* las versiones anteriores de las Directrices de OpenAIRE utilizaban el `vocabulario info:eu-repo-Access-Terms <https://wiki.surfnet.nl/display/standards/info-eu-repo/#info-eu-repo-AccessRights>`_.


Propiedad accessRights (M, 1)
-----------------------------

Use la etiqueta del término del vocabulario como valor.

Atributo uri (M)
----------------

Use el URI del concepto del término del vocabulario.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <datacite:rights rightsURI="http://purl.org/coar/access_right/c_abf2">open access</datacite:rights>

.. _COAR Access Right Vocabulary: http://vocabularies.coar-repositories.org/documentation/access_rights/

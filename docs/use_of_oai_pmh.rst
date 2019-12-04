Uso de OAI-PMH
==============

OpenAIRE es compatible con varios protocolos de transferencia e interfaces de 
recolección de metadatos bibliográficos. A continuación, se describe el uso de uno de 
los principales protocolos, `el protocolo OAI-PMH v2.0<http://www.openarchives.org/OAI/openarchivesprotocol.html>`_,, en el contexto de estas 
directrices y de su perfil de aplicación.

Formato de los metadatos
^^^^^^^^^^^^^^^^^^^^^^^^

OpenAIRE espera que se codifiquen los metadatos de acuerdo al formato de 
metadatos definido en el perfil de aplicación de OpenAIRE. Se recomienda utilizar el 
prefijo de metadatos ``oai_openaire``. Para obtener información sobre cómo usar las 
propiedades individuales, consulte la sección :ref:`application_profile`.


Contenido de los metadatos
^^^^^^^^^^^^^^^^^^^^^^^^^^

OpenAIRE recolecta metadatos de productos científicos de acuerdo con la Política de 
Adquisición de Contenido de OpenAIRE publicada en https://doi.org/10.5281/zenodo.1446407.
Esta incluye metadatos bibliográficos que describen elementos de acceso abierto y no abierto.


Compatibilidad de los agregadores
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Además de repositorios y revistas individuales, también los agregadores (por ejemplo, 
a nivel nacional) pueden ser compatibles con OpenAIRE. En este caso, OpenAIRE 
requiere que el agregador codifique en cada registro de metadatos información 
adicional de procedencia de los proveedores de contenido originales. De acuerdo con 
las `directrices de OAI-PMH <http://www.openarchives.org/OAI/2.0/guidelines-provenance.htm>`_, la información de procedencia debe incluirse bajo el nodo 
del elemento ``about`` del registro OAI, según se muestra en el siguiente ejemplo:

.. code-block:: xml
   :linenos:

    <about>
      <provenance xmlns="http://www.openarchives.org/OAI/2.0/provenance"
      xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xsi:schemaLocation="http://www.openarchives.org/OAI/2.0/provenance
      http://www.openarchives.org/OAI/2.0/provenance.xsd">
        <originDescription altered="true" harvestDate="2012-09-17T14:58:36Z">
          <baseURL>http://dspace.library.uu.nl:8080/dspace-oai/request</baseURL>
          <identifier>oai:dspace.library.uu.nl:1874/218065</identifier>
          <datestamp>2012-01-19T12:38:56Z</datestamp>
          <metadataNamespace>
            http://www.openarchives.org/OAI/2.0/oai_dc/
          </metadataNamespace>
        </originDescription>
      </provenance>
    </about>

Esto significa que se espera que se codifique la información en los siguientes 
elementos (tomado de https://www.openarchives.org/OAI/2.0/guidelines-provenance.htm):

* ``baseURL`` - la ``baseURL`` del repositorio de origen desde donde fue cosechado el registro de metadatos.
* ``identifier`` - el identificador único del ítem en el repositorio de origen desde donde se difundió el registro de metadatos.
* ``datestamp`` - la fecha del registro de metadatos difundido por el repositorio de origen.
* ``metadataNamespace`` - la fecha del registro de metadatos difundido por el repositorio de origen.
* ``originDescription`` - un bloque opcional ``originDescription`` obtenido cuando se cosechó el registro de metadatos. Un conjunto de bloques ``originDescription`` anidados describe la procedencia tras una sucesión de cosechas.

Todo elemento ``originDescription`` debe incluir también los dos siguientes atributos relacionados con el acto de cosecha y cualquier procesamiento posterior:

* ``harvestDate`` - la fecha de  la respuesta OAI-PMH que dio lugar al registro cosechado del repositorio de origen.
* ``altered`` - un valor booleano que debe ser verdadero (true) si el registro cosechado ha sido alterado antes de ser nuevamente diseminado.



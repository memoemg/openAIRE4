.. _dci:identifier:

Identificador de recurso (M)
============================

``datacite:identifier``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

El identificador es una cadena única que identifica un recurso.

**Instrucciones de uso**

Para tener una mejor práctica se recomienda identificar al recurso por medio de una cadena o un número que se ajuste a un sistema de identificación formal. Algunos ejemplos de sistemas de identificación formal incluyen el Identificador Uniforme de Recursos (URI, por sus siglas en inglés), el Localizador Uniforme de Recursos (URL, por sus siglas en inglés), el Identificador de Objeto Digital (DOI, por sus siglas en inglés) y el ``URN:NBN``. También puede ser un URL directo o un URL de redirección, como PURL, HANDLE u otros mecanismos de resolución internacional.

El uso ideal de este elemento es como enlace directo o enlace a una página de salto (una URL persistente) desde ``identifier`` en el registro de metadatos hacia el recurso digital o una página de salto.

Práctica inteligente:

* úsese una URL estable.

**No confundir con**

* :ref:`dci:alternativeIdentifier` (Use ``datacite:alternativeIdentifier`` para enumerar otros identificadores distintos al identificador primario aplicado al mismo recurso).
* :ref:`dci:relatedIdentifier` (Use ``datacite:relatedIdentifier`` para referirse a recursos relacionados).
* :ref:`aire:file` (Use ``oaire:file`` para señalar el recurso descrito por estos metadatos, por ejemplo, el archivo de texto completo).
* :ref:`dc:source` (Use ``dc:source`` para las citas bibliográficas del recurso original).

Propiedad identifier (M, 1)
---------------------------

Utilice el enlace del identificador como valor.

Atributo identifierType (M)
---------------------------

Tipo de identificador (ocurrencias: 1).

**Valores permitidos, ejemplos y otras restricciones**

.. include:: vocabularies/identifiertype.rst

.. note::
   A diferencia de DataCite, OpenAIRE permite DOI y otros tipos de identificadores.

Ejemplo
~~~~~~~

En este ejemplo, el identificador handle redirige a la página de salto. Una página de salto es un buen lugar al que se puede referir. El usuario final tiene la oportunidad de ver más información sobre el(los) objeto(s) que ha encontrado, ver el contexto y acceder a  los otros servicios que el repositorio local ofrece:

.. code-block:: xml
   :linenos:

   <datacite:identifier identifierType="Handle">http://hdl.handle.net/1234/5628</datacite:identifier>

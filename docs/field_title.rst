.. _dci:title:

.. _dci:title_title:

Título (M)
==========

``datacite:title``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Occurrencia: 1-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Nombre o título por el que se conoce al recurso.

**Valores permitidos, ejemplos y otras restricciones**

Texto libre.

**Observaciones**

* Adaptado de `DataCite MetadataKernel`_ v4.1

Propiedad title (M, 1-n)
-----------------------

Utilice el nombre del título como valor. Repita esta propiedad para los diferentes tipos o idiomas de los títulos.

Atributo lang (O)
------------------

Idioma del título (occurrence: 0-1)

Use el atributo ``xml:lang`` para indicar el idioma del título. El valor del atributo debe elegirse de IETF BCP 47, el `Registro de Subetiquetas de Idiomas de IANA <http://www.iana.org/assignments/language-subtag-registry>`_.


Atributo titleType (O)
-----------------------

Tipo de título (occurrences: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

.. include:: vocabularies/titletype.rst


Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

    <datacite:titles>
        <datacite:title xml:lang="en-US">
         National Institute for Environmental Studies and Center
         for Climate System Research Japan
        </datacite:title>
        <datacite:title xml:lang="en-US" titleType="Subtitle">A survey</datacite:title>
    </datacite:titles>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/
.. _dci:datePublication:

Fecha de publicación (M)
========================

``datacite:date``

Cardinalidad
~~~~~~~~~~~~

*Obligatorio*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Fecha asociada a un evento en el ciclo de vida del recurso. Normalmente, la fecha se asocia con la creación o disponibilidad del recurso. La mejor práctica recomendada para codificar el valor de la fecha se define en un perfil de la norma `ISO 8601 [W3CDTF] <https://www.iso.org/iso-8601-date-and-time-format.html>`_ y sigue el formato ``AAAA-MM-DD``.

**Instrucciones de uso**

La fecha se debe formatear de acuerdo con las reglas de codificación de W3C para las fechas y horas:

**Fecha completa:**

``AAAA-MM-DD`` (por ejemplo, 1997-07-16)

donde:

* ``AAAA`` [año de cuatro dígitos] es ''obligatorio''
* ``MM`` [mes de dos dígitos (01=enero, etc.)] es ''opcional''
* ``DD`` [día de dos dígitos (del 01 al 31)] es ''ociional''

**Sólo una fecha - Fecha de publicación:**

Los sistemas de repositorios a menudo tienen múltiples campos de fecha que sirven para diferentes propósitos: fecha de creación, publicación, modificación, promoción, etc. Preferiblemente, desde la perspectiva del usuario, la fecha más lógica y significativa es la fecha de publicación. 

**Sin fecha de publicación disponible:**

Si no se cuenta con una fecha de publicación, use cualquier otra fecha disponible. Es mejor usar una fecha que no usar ninguna.

**Adiciones a la marca de fecha:**

Las adiciones como "tiempo Zulu" NO deben ser parte de los metadatos.

**Fechas difusas:**

Para las fechas difusas, use el año lógico que más represente ese período, por ejemplo, ``1650`` en lugar de ``siglo XVII``.

Para expresar más sobre ese período temporal, se puede usar el campo ``dc:coverage``. Un período temporal se puede expresar de manera estándar cuando se define con precisión (consulte la sección sobre :ref:`dc:coverage`) o cuando sea "difuso" o no sea claro al usar expresiones de texto libre. El proveedor de servicios puede ordenar las fechas según los estándares de fechas tales como W3CDTF. Dado que no hay una norma para fechas difusas para los términos como "Renacimiento" o "Siglo XVII", simplemente no aparecerán en los resultados de las consultas basadas en la fecha.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element date`_
* esta versión del perfil de aplicación adopta el elemento date en combinación con el atributo *dateType* de `DataCite MetadataKernel`_ v4.1.

Propiedad date (M, 1)
---------------------

Utilice la fecha de publicación como valor.

Atributo dateType (M)
---------------------

Tipo de fecha. Elija del uso de vocabulario del  :ref:`tipo de fecha <vocab:datetype_datetype>` el término controlado ``Issued`` para indicar la fecha de publicación.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

     <datacite:dates>
          <datacite:date dateType="Issued">2000-12-25</datacite:date>
     </datacite:dates>

.. _DRIVER Guidelines v2 element date: https://wiki.surfnet.nl/display/DRIVERguidelines/Date
.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

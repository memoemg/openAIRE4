.. _aire:licenseCondition:

Condición de la licencia (R)
============================

``oaire:licenseCondition``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Información sobre los derechos de licencia mantenidos sobre el recurso.

**Instrucciones de uso**

Normalmente, un elemento ``licenseCondition`` tiene una declaración de la administración de derechos para el uso del objeto o una referencia a un servicio que proporcione dicha información. La información sobre los derechos a menudo abarca los Derechos de Propiedad Intelectual (DPI), los Derechos de Autor y varios Derechos de Propiedad. Es preferible referirse a un servicio de derechos donde al usuario final se le expliquen los derechos de reutilización mediante el uso de un URL. Por ejemplo, la organización Creative Commons ha creado identificadores URI para sus diferentes licencias en distintas jurisdicciones. Esto se puede aplicar para crear licencias de uso legibles por máquina.

Propiedad licenseCondition (R, 1)
---------------------------------

Utilice el nombre de la licencia como valor.

Atributo uri (MA)
-----------------

El URL proporciona la ubicación donde se puede leer la licencia. Con las licencias de Creative Commons, el tipo de licencia se puede reconocer en el mismo nombre del URL. Una razón a favor de tener la licencia ligada a una URL de esta manera es que la puede leer una máquina.

Atributo startDate (MA)
-----------------------

Este atributo indica la fecha en que la licencia entra en vigor. La mejor práctica recomendada para codificar el valor de la fecha se define en un perfil de la norma ISO 8601 [W3CDTF] y sigue el formato ``AAAA-MM-DD``.



Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <!-- example 1 -->
   <oaire:licenseCondition startDate="2019-02-01" uri="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial</oaire:licenseCondition>


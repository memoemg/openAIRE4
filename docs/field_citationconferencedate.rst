.. _aire:citationConferenceDate:

Fecha de la conferencia de la cita (R)
======================================

``oaire:citationConferenceDate``

Cardinalidad
~~~~~~~~~~~~

*Recomendado*

*Ocurrencia: 0-1*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Se refiere a la fecha en la que tuvo lugar la conferencia. Esta propiedad se considera parte de la cita bibliográfica. La mejor práctica recomendada para codificar el valor de la fecha se define en un perfil de la norma `ISO 8601 [W3CDTF] <https://www.iso.org/iso-8601-date-and-time-format.html>`_ y sigue el formato ``AAAA-MM-DD``.

**Instrucciones de uso**

La fecha se debe formatear de acuerdo con las reglas de codificación de W3C para las fechas y horas:

**Fecha completa:**

``AAAA-MM-DD`` (e.g. 1997-07-16)

donde:

* ``AAAA`` [año de cuatro dígitos]
* ``MM`` [mes de dos dígitos (01=enero, etc.)]
* ``DD`` [día de dos dígitos (del 01 al 31)]

Propiedad citationConferenceDate (R, 0-1)
----------------------------------------

Use la *fecha única* or *fecha de inicio* y *fecha de finalización* como valores siguiendo estos patrones:

* ``AAAA-MM-DD`` [*fecha única*]
* ``AAAA-MM-DD - AAAA-MM-DD`` [*fecha de inicio* - *fecha de finalización*]

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:

   <oaire:citationConferenceDate>2013-10-22</oaire:citationConferenceDate>

.. code-block:: xml
   :linenos:

   <oaire:citationConferenceDate>2013-09-22 - 2013-09-26</oaire:citationConferenceDate>

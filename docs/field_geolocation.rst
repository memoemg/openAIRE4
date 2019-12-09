.. _dci:geolocation:

Ubicación geográfica (O)
========================

``datacite:geoLocation``

Cardinalidad
~~~~~~~~~~~~

*Opcional*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Región espacial o nombre del lugar donde se recopilaron los datos o sobre los que se enfocaron los datos.

Propiedad geoLocation (O, 0-n)
------------------------------

Repita esta propiedad para indicar varias ubicaciones diferentes.

.. _d:geolocationpoint:

Subpropiedad geoLocationPoint (O)
*********************************

Punto de ubicación en el espacio (ocurrencia: 0-1).

Un punto contiene un único par de latitud-longitud.

Véanse las :ref:`d:geolocation_instructions`.

pointLongitude (M)
++++++++++++++++++

Dimensión longitudinal del punto (ocurrencia: 1).

Es obligatorio si se usa *geoLocationPoint*.

pointLatitude (M)
+++++++++++++++++

Dimensión latitudinal del punto (ocurrencia: 1).

Es obligatorio si se usa *geoLocationPoint*.

.. _d:geolocationbox:

Subpropiedad geoLocationBox (O)
*******************************

Límites espaciales de un lugar o un cuadro (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Un cuadro se define por dos puntos geográficos: esquina inferior izquierda (normalmente suroeste), esquina superior derecha (normalmente noreste). Cada punto está definido por su longitud y latitud.

Véanse las :ref:`d:geolocation_instructions`.

westBoundLongitude (M)
++++++++++++++++++++++

Dimensión longitudinal occidental del cuadro. Es obligatorio si se usa *geoLocationBox*.

eastBoundLongitude (M)
++++++++++++++++++++++

Dimensión longitudinal oriental del cuadro. Es obligatorio si se usa *geoLocationBox*.

southBoundLatitude (M)
++++++++++++++++++++++

Dimensión latitudinal sur del cuadro. Es obligatorio si se usa *geoLocationBox*.

northBoundLatitude (M)
++++++++++++++++++++++

Dimensión latitudinal norte del cuadro. Es obligatorio si se usa *geoLocationBox*.

.. _d:geolocationplace:

Subpropiedad geoLocationPlace (O)
*********************************

Descripción de una ubicación geográfica (ocurrencias: 0-1).

**Valores permitidos, ejemplos y otras restricciones**

Texto libre. Úsese para describir una ubicación geográfica.

Subpropiedad geoLocationPolygon (O)
***********************************

Área de un polígono trazado, definida por un conjunto de puntos y líneas que conectan los puntos en una cadena cerrada (ocurrencias: 0-n).

polygonPoint (M)
++++++++++++++++

Punto de ubicación en un polígono (ocurrencias: 4-n). Es obligatorio si se usa *geoLocationPolygon*.

pointLongitude (M)
^^^^^^^^^^^^^^^^^^

Dimensión longitudinal del punto (ocurrencia: 1). Es obligatorio si se usa *polygonPoint*.


pointLatitude (M)
^^^^^^^^^^^^^^^^^

Dimensión latitudinal del punto (ocurrencia: 1). Es obligatorio si se usa *polygonPoint*.

inPolygonPoint (O)
++++++++++++++++++

Para cualquier área delimitada que sea mayor que la mitad de la Tierra, defina un punto (aleatorio) en el interior.

pointLongitude (M)
^^^^^^^^^^^^^^^^^^

Dimensión longitudinal del punto (ocurrencia: 1). Es obligatorio si se usa *inPolygonPoint*.

pointLatitude (M)
^^^^^^^^^^^^^^^^^

Dimensión latitudinal del punto (ocurrencia: 1). Es obligatorio si se usa *inPolygonPoint*.

.. _d:geolocation_instructions:

Instrucciones detalladas de uso
*******************************
Utilice las coordenadas WGS 84 (Sistema Geodésico Mundial). Use solo números decimales para las coordenadas. Las longitudes van de -180 a 180 (donde 0 es Greenwich, los números negativos son al oeste y los positivos al este), mientras que las latitudes van de -90 a 90 (donde 0 es el ecuador y los números negativos son al sur y los positivos al norte).

**Observaciones**

* adaptado de `DataCite MetadataKernel`_ v4.1

Ejemplo
~~~~~~~
.. code-block:: xml
   :linenos:

   <datacite:geoLocations>
     <datacite:geoLocation>
       <datacite:geoLocationPlace>Atlantic Ocean</datacite:geoLocationPlace>
       <datacite:geoLocationPoint>
        	<datacite:pointLongitude>31.233</datacite:pointLongitude>
       		<datacite:pointLatitude>-67.302</datacite:pointLatitude>
       </datacite:geoLocationPoint>
       <datacite:geoLocationBox>
       		<datacite:westBoundLongitude>-71.032</datacite:westBoundLongitude>
        	<datacite:eastBoundLongitude>-68.211</datacite:eastBoundLongitude>
       		<datacite:southBoundLongitude>41.090</datacite:southBoundLongitude>
       		<datacite:northBoundLongitude>42.893</datacite:northBoundLongitude>
       </datacite:geoLocationBox>
     </datacite:geoLocation>
   </datacite:geoLocations>

.. _DataCite MetadataKernel: http://schema.datacite.org/meta/kernel-4.1/

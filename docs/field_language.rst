.. _dc:language:

Idioma (MA)
===========

``dc:language``

Cardinalidad
~~~~~~~~~~~~

*Es obligatorio cuando corresponda*

*Ocurrencia: 0-n*

Definición e instrucciones de uso
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

**Definición según la Iniciativa de Metadatos de Dublin Core (DCMI, por sus siglas en inglés)**

Lenguaje del contenido intelectual del recurso.

**Instrucciones de uso**

Se refiere a un recurso específico (una instancia de la producción científica) escrito en uno o más lenguajes humanos. En estos casos, todos los idiomas usados se utilizan en el elemento DC ``language``. Si un recurso específico (una instancia de la producción científica) está escrito en un lenguaje humano y se traduce a otros lenguajes humanos, cada traducción tiene su propia instancia.

Recomendación: tomar valores de una de las siguientes listas: 

* IETF BCP 47, el `Registro de subetiquetas de idioma de la IANA (*IANA Language Subtag Registry*) <http://www.iana.org/assignments/language-subtag-registry>`_
* ISO 639-x,  donde x puede ser 1, 2 o 3. Mejor práctica: usamos la norma ISO 639-3 y al hacerlo seguimos lo expuesto en: http://www.sil.org/iso639-3/

De ser necesario, repita este elemento para indicar varios idiomas.

Si las normas ISO 639-2 y 639-1 son suficientes para los contenidos de un repositorio, pueden usarse en forma alternativa. Dado que existe una correspondencia única entre sus valores, se pueden convertir sus valores durante un proceso de agregación.

**Observaciones**

* introducido en `DRIVER Guidelines v2 element language`_

Propiedad language (MA, 0-n)
----------------------------

Utilice el código idioma como valor.

Ejemplo
~~~~~~~

.. code-block:: xml
   :linenos:


   <dc:language>eng</dc:language>
   <dc:language>deu</dc:language>
   <dc:language>nld</dc:language>
   <dc:language>nld/dut</dc:language>
   <dc:language>dut</dc:language>
   <dc:language>nl</dc:language>

.. _DRIVER Guidelines v2 element language: https://wiki.surfnet.nl/display/DRIVERguidelines/Language

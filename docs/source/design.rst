📐 Design
===========================

Electronic schematics
---------------------
.. image:: ../../Documentation/Schematics/Schematic_1.png
    :width: 30%

.. image:: ../../Documentation/Schematics/Schematic_2.png
    :width: 30%

.. image:: ../../Documentation/Schematics/Schematic_3.png
    :width: 30%

:download:`Download PDF <../../Documentation/Schematics/Schematic.pdf>`

.. _pcb:

:term:`PCB`
----------

.. raw:: html

    <iframe src="_static/ibom.html" height="800px" width="100%"></iframe>


.. _dock:

Dock stand
-----------------------

.. Caution::
    The following enclosure was designed for 5050100 (100x50x5mm) 4000mAh LiPo battery. The recommended battery wouldn't fit in this enclosure.



.. image:: ../../Enclosure/Render.png
    :width: 100%


 - :download:`Bottom <../../Enclosure/Bottom.stl>`
 - :download:`Top <../../Enclosure/Top.stl>`

 
Technical Specifications
--------------------------

Microcontroller 
^^^^^^^^^^^^
.. list-table:: 
    :widths: 50 80
    :stub-columns: 1

    * - Module
      - ESP32-S2-MINI-1
    * - SoC
      - Xtensa® singlecore 32-bit LX7 up to 240MHz
    * - Flash
      - 4MB
    * - PSRAM
      - 2MB

Power
^^^^^^^^^^^^

.. list-table:: 
    :widths: 50 80
    :stub-columns: 1

    * - Battery 
      - LiPo 3.7 V 5000 mAh
    * - Input (USB/Solar panel)
      - 5V @ 500mA


Features
^^^^^^^^^^^^

.. list-table:: 
    :widths: 50 80
    :stub-columns: 1

    * - Interface 
      - USB Type C 
    * - 
      - 2.4GHz WiFi 
    * - 
      - UART
    * - Display
      - 7.5" B&W E-Ink display 
    * - 
      - 7.3" ACeP 7-Color E-Ink Display
    * - Sensors
      - BMP280 air temperature & pressure (digital :math:`I^2C`)
    * - 
      - MAX17048 battery voltage level sensor (digital :math:`I^2C`)


Dimensions
^^^^^^^^^^^^

.. list-table:: 
    :widths: 50 80
    :stub-columns: 1

    * - Size 
      - 100x30mm
    * - Weight
      - 15g

Environment
^^^^^^^^^^^^

.. list-table:: 
    :widths: 50 20 20 20 20 20
    :header-rows: 1
    :stub-columns: 1

    * - Parameter
      - Symbol
      - Min.
      - Typ.
      - Max.
      - Unit
    * - Working temperature [1]_
      - :math:`T_{amb}`
      - 0
      - 25 
      - 60
      - *°C*
    * - Storage temperature [1]_
      - :math:`T_{amb}`
      - 0
      - 25 
      - 60
      - *°C*

.. [1] Based on components datasheets.



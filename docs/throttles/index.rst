.. include:: /include/include.rst
.. include:: /include/include-l1.rst
.. include:: /include/include-throttles.rst
|EX-THROTTLES-LOGO|

***********************
Throttles (Controllers)
***********************

This page contains lists of compatible Throttles (Controllers) that currently support the |EX-CS|.  They are listed two ways:

.. sidebar:: 

  .. contents:: On this page
    :depth: 2
    :local:


* :ref:`By Client Technology <throttles/index:throttles - by client technology>`  (e.g. Android, iOS, Web Browser, PC)
* :ref:`By Communication Technology <throttles/index:throttles - by communication technology>` (e.g. |DCC-EX Native Commands|, wiThrottle Protocol)

|conductor|

For an more introductory overview of throttles and how to choose one, please read the :doc:`Getting Started - Throttles Page </ex-commandstation/get-started/controllers>` 

|tinkerer| |engineer|

For additional options for throttles and how to choose one, please read the :doc:`Advanced Options - Throttles Page </ex-commandstation/advanced-setup/controllers>`

----

Throttles - By Client Technology
================================

Web Browser (Windows, OSX, Linux)
---------------------------------

- :doc:`EX-Web-Throttle (Web Browser) </ex-webthrottle/index>`

Android (Phones and Tablets)
----------------------------

- :doc:`Engine Driver (Android)<software/engine-driver>`
- :doc:`DCCpp CAB (android) <software/dccpp-cab>`
- :doc:`Cab Engineer: DCC Throttle (Andriod) <software/cab-engineer>`
- :doc:`DigiTrainsPro (Android, iOS, Windows) <software/digitrainspro>` *- Requires JMRI*
- :doc:`RtDtive DCC++ (Android) <software/rtdrive-dccpp>`

Apple iOS (Phones and Tablets)
------------------------------

- :doc:`Locontrol (iOS) <software/locontrol>` *- Requires JMRI*
- :doc:`WiThrottle (iOS) <software/withrottle>`
- :doc:`SRCP Client (iOS) <software/srcpclient>`
- :doc:`Train Driver (iOS) <software/train-driver>`
- :doc:`DigiTrainsPro (Android, iOS, Windows) <software/digitrainspro>` *- Requires JMRI*


Dedicated Hardware
------------------

- :doc:`miniThrottle (Physical) <hardware/minithrottle>`
- :doc:`WiTcontroller (Physical) <hardware/witcontroller>`
- :doc:`DccExController (Physical) <hardware/dccexcontroller>`
- :doc:`TCS UWT-50 (Physical) <hardware/uwt50>`
- :doc:`Elgato Stream Deck (Physical) <hardware/streamdeck>`
- :doc:`DCC-EX Native command library - DCCEXProtocol </throttles/native-protocol-library>`

Personal Computers
------------------

- :doc:`EX-WebThrottle </ex-webthrottle/index>`  *(Web Browser)*
- :doc:`JMRI (Windows, iOS, Linux) <software/jmri>`
- :doc:`DigiTrainsPro (Android, iOS, Windows) <software/digitrainspro>` *- Requires JMRI*
- :doc:`Train Throttle <software/train-throttle>`
- :doc:`Railroad Automation <software/railroad-automation>` *- Requires IoTT Red Hat*

Note: The Android throttle apps listed above can be made to made to run on Windows PCs. See :doc:`Running Android apps on Microsoft Windows <software/android-apps-on-windows>`.


----

Throttles - By Communication technology
=======================================

|EX-CS| can use a number of different technologies to communicate with a throttle. While each technology has advantages and disadvantages, none is substantially better that the others.

General
-------

- :doc:`WiThrottle Server, Web Server, DCC-EX Native Commands Explained <protocols>`
- :doc:`connect_wifi_throttle_via_usb`

DCC-EX (DCC-EX Native Commands)
-------------------------------

- :doc:`EX-WebThrottle </ex-webthrottle/index>`
- :doc:`Engine Driver (Android)<software/engine-driver>`
- :doc:`SRCP Client (iOS) <software/srcpclient>`
- :doc:`miniThrottle (Physical) <hardware/minithrottle>`
- :doc:`JMRI <software/jmri>`
- :doc:`RtDtive DCC++ (Android) <software/rtdrive-dccpp>`
- :doc:`DCCpp CAB (Android) <software/dccpp-cab>`
- :doc:`DccExController (Physical) <hardware/dccexcontroller>`
- :doc:`DCC-EX Native command library - DCCEXProtocol <throttles/native-protocol-library>`

WiThrottle Protocol Based Throttles
-----------------------------------

- :doc:`Engine Driver (Android)<software/engine-driver>`
- :doc:`Cab Engineer: DCC Throttle (Andriod) <software/cab-engineer>`
- :doc:`WiThrottle (iOS)<software/withrottle>`
- :doc:`SRCP Client (iOS) <software/srcpclient>`
- :doc:`Train Driver (iOS) <software/train-driver>`
- :doc:`miniThrottle (Physical) <hardware/minithrottle>`
- :doc:`WiTcontroller (Physical) <hardware/witcontroller>`
- :doc:`TCS UWT-50 (Physical) <hardware/uwt50>`
- :doc:`Elgato Stream Deck (Physical) <hardware/streamdeck>`

USB Based Throttles
-------------------------------

- :doc:`EX-WebThrottle </ex-webthrottle/index>`
- :doc:`myBluePillThrottle <hardware/mybluepillthrottle>`
- Also see: :doc:`connect_wifi_throttle_via_usb`

JMRI Web Server Based Throttles
-------------------------------

- :doc:`Locontrol (iOS) <software/locontrol>`
- :doc:`DigiTrainsPro (Android) <software/digitrainspro>`

----

Table - Command Suites and Throttles Crossreference 
===================================================

.. table::
    :width: 100%
    :widths: 10 8 8 10 8 8 8 8 8 8 8 8
    :align: center
    :class: command-table

  ========= ============ =============== =========== ========== ========== ========= ===== ========= ========= ======= =======
    Train                        Technology Stack                                           Form Factor
  --------- --------------------------------------------------- --------------------------------------------------------------
   Project   Connection   Communication     User       Also       Device        Mobile Handhelds        Personal Computer
  --------- ------------ --------------- ----------- ---------- ---------- ------------------------- -------------------------
    Name        Type        Protocol      Interface   Requires   Physical   Android   iOS   Windows   Windows   MacOS   Linux
  ========= ============ =============== =========== ========== ========== ========= ===== ========= ========= ======= =======


.. csv-table::
    :width: 100%
    :widths: 10 8 8 10 8 8 8 8 8 8 8 8
    :stub-columns: 1
    :align: center
    :class: command-table

  JMRI,Network,Native,Command Suite,,,✔ (Web),✔ (Web),✔ (Web),✔ (App),✔ (App),✔ (App)
  Railroad Auto-mation,Network or LocoNet,LocoNet,Command Suite,IoTT Red Hat,,✔ (Web),✔ (Web),✔ (Web),✔ (App),✔ (App),✔ (App)
  EX-Web Throttle,USB/Serial,Native,Web,,,,,,✔,✔,✔
  Engine Driver,Network,Native,App,,,✔,,,,,
  DCCpp CAB,Network,Native,App,,,✔,,,,,
  Cab Engineer: DCC Throttle,Network,WiThrottle,App,,,✔,,,,,
  RtDtive DCC++,Network,Native,App,,,✔,,,,,
  DigiTrains Pro,Network,JMRI Web,App,JMRI,,✔,✔,,✔,,
  Locontrol,Network,JMRI Web,App,JMRI,,,✔,,,,
  WiThrottle,Network,WiThrottle,App,,,,✔,,,,
  SRCP Client,Network,Native,App,,,,✔,,,,
  Train Driver,Network,Native,App,,,,✔,,,,
  Train Throttle,Network,WiThrottle,App,,,,,✔,✔,,
  mini Throttle,Network or Serial,Native,Device,,✔,,,,,,
  WiT controller,Network,WiThrottle,Device,,✔,,,,,,
  TCS UWT Throttles,Network,WiThrottle,Device,,✔,,,,,,
  Elgato Stream Deck,Network,Native,Device,PC or Raspberry Pi,✔,,,,,,
  LocoNet-Compatible Throttles,LocoNet,LocoNet,Device,IoTT Red Hat,✔,,,,,,


.. csv-table:: Legend
    :widths: auto
    :stub-columns: 1
    :align: left
    :delim: =
    :class: command-table

  Net = Wifi or LAN networks
  Free / paid = Both Free and Paid versions are available.  The free version might be limited in features.
  Native = Uses the Native DCC-EX command / command protocols
  WiT = Uses the WiThrottle command protocol
  Web = Requires the use of a web browser
  Win = Windows 7 and above

Note: The Android throttle apps listed above can be made to made to run on Windows PCs. See :doc:`Running Android apps on Microsoft Windows <software/android-apps-on-windows>`.

----

Reference
=========

- :doc:`Technical Reference for Throttle Developers <tech-reference>`
- :doc:`DCC-EX Native command library - DCCEXProtocol </throttles/native-protocol-library>`

.. toctree::
    :maxdepth: 3
    :hidden:
    
    protocols
    software/index
    hardware/index
    connect_wifi_throttle_via_usb
    tech-reference
    DCC-EX Native command library </throttles/native-protocol-library>

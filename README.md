# Workshop Industrial edge team NL ![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)

Edge workshop with fakeplc connector
In plaats van het verbinden met een s7 connector verbinden wij met de fakeplc connectorDeze connector simuleert dezelfde Data zoals de tank applicatie deze produceert. 
Based on [The tank application](https://github.com/industrial-edge/miscellaneous/tree/main/tank%20application)

Beschikbare demos:

* Archiving and visualisation (zonder hmi_nextbottle) 
  ** databus, influx, grafana
  
* Iot gateway 
  ** databus, cloud connector, flow creator.

* Data service getting started 
  ** dabus, Data service

* Notifier getting started 
  ** databus, dataservice, notifier

* Performance insight getting started 
  ** databus, dataservice, performance insight

* Performance insight oee dashboard 
  ** Dataservice, Databus, Perf insight.

* Energy manager getting started 
  ** Dataservice, Databus, Energy manager.

Gebruikte tags:
GDB.signals.tankSignals.actLevel
GDB.signals.tankSignals.actTemperature
GDB.process.numberProduced
GDB.process.numerFaulty
GDB.operate.machineState
GDB.signals.energySignals.energyConsumptionFillingTank
GDB.signals.energySignals.waterConsumptionFillingTank
GDB.signals.energySignals.energyConsumptionHeatingTank
GDB.signals.energySignals.energyConsumptionFillingBottle

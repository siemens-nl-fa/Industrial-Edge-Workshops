# Configuration
- [Configure Data Service](#configure-data-service) 
  - [Configure an asset with variables](#configure-an-asset-with-variables)
- [Configure Performance Insight](#configure-performance-insight)
    - [Configure a dashboard](#configure-a-dashboard)
    - [Configure widgets](#configure-widgets)
    - [Configure KPIs](#configure-KPIs)
		
# PREConfigured PLC Connection

To read data from the PLC and provide the data, we will use OPC UA Connector to establish connection with the PLC.
The OPC UA Connector sends the data to the Databus, where the Data Service app can collect what is needed. The Performance Insight app is extremely dependent on a properly configured data service app.
In order to build this infrastructure, these apps must be configured properly:

- OPC UA Connector
- Databus
- Data Service
- Performance Insight

 <p align="center"><kbd><img src="graphics/performanceinsight.PNG"/></kbd></p>

# Configure Data Service

In your IED Web UI open the app Data Service.

Hint: If an error screen appears saying "...unauthorized...", please restart the Data Service app, wait a moment and try again to open it.

## Configure an asset with variables

On the left bar click the icon "Assets & Connectivity". For the "edge" asset you can add child assets as needed.

Choose "Multiple variables" on the right side to add tags.

The required tank application requires some variables, but you can add them all.

<p align="center"><kbd><img src="graphics/assestsandconnect.png"/></kbd></p>



# Configure Performance Insight

In your IED Web UI open the app Performance Insight.

<p align="center"><kbd><img src="graphics/Logo.PNG" /></kbd></p>

Hint: When opening the application for the first time a lincese message might pop up (no relationship to IE Hub). Just accept the message and start using the application

## Configure a dashboard

On the my plant panel the dashboard overview will show the option to Add a new dashboard (operating at the highest hirerchical level configured in data service)

<p align="center"><kbd><img src="graphics/Assets dashboard.PNG" /></kbd></p>

Insert a dashboard name and select the time period that should be display per default for all signals

<p align="center"><kbd><img src="graphics/Adddashboard.PNG" /></kbd></p>

## Configure widgets

When configuring a widget, Performance Insight offers the following types:

<p align="center"><kbd><img src="graphics/widget types.PNG" /></kbd></p>

The standard widget configuration has to select some parameters

<p align="center"><kbd><img src="graphics/Parameter of INSIGHT.PNG" /></kbd></p>

The following steps are to define details and display options 

In case of a Gauge Widget an additional dialog will appear with the display boundaries parametrization

<p align="center"><kbd><img src="graphics/Detail Insight.PNG" /></kbd></p>

The first widget is a gauge display for the actual production quantity (with its respective warning and alarming levels)

<p align="center"><kbd><img src="graphics/Quality insight.PNG" /></kbd></p>

Several widgets have been configured as single value display (with Min, Avg and Max Values)

<p align="center"><kbd><img src="graphics/Tempfaultvalues.PNG" /></kbd></p>

Another configured widget is a diagram display for the actual tank level

<p align="center"><kbd><img src="graphics/Performance_Insight_Diagram_Widget.png" /></kbd></p>

The last used widget on this application example is a Gantt diagram. The first step is to configure a status mapping

<p align="center"><kbd><img src="graphics/Machinestatus.PNG" /></kbd></p>

Afterwards the Widget has to be added. The Gantt Overview will be displayed on the dashboard

<p align="center"><kbd><img src="graphics/performance-insight-gantt-overview.png" /></kbd></p>

By clicking the detailed view icon, a detailed Gantt diagram will be shown (more visible data)



## Configure KPIs

Additional values (also named KPIs) can be calculated out of the existing variables.


When configuring a widget, an instance can be created, select a gauge and press next:

<p align="center"><kbd><img src="graphics/Parameter of INSIGHT_2.PNG" /></kbd></p>

In order to calculate the production availability a KPI instance to be created.

<p align="center"><kbd><img src="graphics/Performance_Insight_KPI_Gauge_Widget_2.png" /></kbd></p>

create new KPI instance with the following parameters, then save.
<p align="center"><kbd><img src="graphics/KPI instance_2.PNG" /></kbd></p>
<p align="center"><kbd><img src="graphics/KPI instance_3.PNG" /></kbd></p>


This quality availability KPI has been displayed using a gauge widget (frist widget mentioned). KPI has been instanced within a widget

<p align="center"><kbd><img src="graphics/Performance_Insight_Gauge_Widget_2.png" /></kbd></p>

From there Fill in the rest and create widget.
# Data collection tools

## ODK
`open source` `free (as in freedom)`

[https://getodk.org/](https://getodk.org/)

ODK is a suite of open source tools that help organizations collect and manage data. It consists of:
- **ODK Collect** - open source Android app for **data collection** that replaces paper forms used in survey-based data gathering.
- **ODK Central** - the **ODK server** that manages user accounts and permissions, stores form definitions, and allows data collection clients like ODK Collect to connect to it for form download and submission upload.
- **ODK Build** - a drag-and-drop **form designer**.

A common workflow using ODK:
- Create survey forms using the XLSForm standard in Excel or Google Sheets.
- Upload forms to an ODK Central server.
- Download forms into ODK Collect on an Android device.
- Use Collect to fill out forms with participants.
- Upload survey data from Collect to Central.
- Analyze or export data from Central.

Learn more about it from the [ODK Documentation](https://docs.getodk.org/).

## ODK-X
`open source` `free (as in freedom)`

[https://odk-x.org/](https://odk-x.org/)

ODK-X is another free and open source toolkit to come out of the Open Data Kit project—the same one that created ODK. Compared to ODK, ODK-X is less mature but it is a more flexible and more complex tool suite.

ODK-X allows you to create your own data management applications consisting of survey forms and Javascript-based apps that can render a fully customizable user interface to gather, manage, and visualize data on an Android device.

The ODK-X Tool Suite consists of:

- **ODK-X Survey**- a customizable **data collection** application.
- **ODK-X Tables** - a **data curation and visualization** application that can also run custom-built data collection workflows.
- **ODK-X Services** - an application for **user authentication and data synchronization** between the ODK-X applications.
- **ODK-X Cloud Endpoints** - a **cloud server** to host data and application files, and to support bi-directional data synchronization across mobile devices.
- **ODK-X Suitcase** - a **desktop tool for synchronizing data** with a cloud endpoint.
- **ODK-X Application Designer** - a **design environment** for creating, customizing, and previewing your forms, data curation, and visualization applications. This is where you **build your ODK-X applications**.

A common data collection workflow using ODK-X:
- ODK-X Application Designer for data collection form creation
- ODK-X Survey for data collection
- ODK-X Services for data sync and database access
- ODK-X Cloud Endpoints for data and application files cloud server

Learn more about it from the [ODK-X Documentation](https://docs.odk-x.org/).


## KoBoToolbox
`open source` `free (as in freedom)` 

[https://www.kobotoolbox.org/](https://www.kobotoolbox.org/)

KoBoToolbox is a suite of free and open source tools for field data collection for use in challenging environments.

It allows you to:
- **Design forms quickly and easily** using a Form Builder
- **Collect data** online and offline via an Android app (KoBoCollect) or on any modern web browser (Enketo).
- **Analyze and manage data** through summary reports, graphs, tables, and maps.

Aside from deploying your own server, KoBoToolbox has two publicly-available instances that you can use:
- Humanitarian Server hosted by UN Office for the Coordination of Humanitarian Affairs (OCHA)
- Non-Humanitarian Server hosted by KoboToolbox

Learn more about it from the [KoBoToolbox Documentation](https://support.kobotoolbox.org/). 

## QField
`open source` `free (as in freedom)` `geospatial`

[https://qfield.org/](https://qfield.org/)

QField is a free and open source application that allows you to bring your QGIS project on the field. It works together with QFieldCloud and QFieldSync so that you can efficiently work on your GIS data outdoors.

With QField, you can:
- Create a project in QGIS on your desktop.
- Collect the data needed for your project on the field.
- Sync, edit, and manage the data you collected back into QGIS.

Learn more about it from the [QField Documentation](https://docs.qfield.org/).

## Mergin Maps
`open source` `free (as in freedom)` `geospatial`

[https://merginmaps.com/](https://merginmaps.com/)

Mergin Maps allows you to capture geospatial information easily through your mobile or tablet then share it with your team for seamless collaboration. It consists of the QGIS Mergin plugin, Mergin Maps Cloud, and Mergin Maps input. 

With Mergin Maps, you can:
- Setup your GIS project on QGIS
- Capture the data you need easily on mobile or tablet using the Mergin Maps Input app for iOS and Android
- Store and track changes to your geodata
- Integrate the data you collected into QGIS

Learn more about it from the [Mergin Maps Documentation](https://merginmaps.com/docs/).
---
uid: SetUpPowerBI
---

# Power BI Connector setup

You must install the AVEVA Data Hub Power BI Connector to retrieve data views for use with Microsoft Power BI.

## System requirements

The following are required before you install and use AVEVA Data Hub Power BI Connector.

- Operation Systems: Windows 10, Windows Server 2012 R2, Windows 8.1, Windows Server 2016, Windows Server 2019

- For desktop installation: Microsoft Power BI Desktop 2.91.884.0 or later

- For on-premises Data Gateway installation: Microsoft Power BI On-premises Data Gateway 3000.89.6 or later

- Microsoft Edge WebView 2 Runtime

- A user account with Administrator privileges to install AVEVA Data Hub Power BI Connector on a local machine.

## Download Power BI Connector

1. In the left pane, select **Analytics** > **Data Views**.

2. Select **More options** ![More options icon](../../_icons/default/dots-vertical.svg) > **Download Power BI Connector**.

3. On the `Power BI Connector Installer Download` window, select **Download**. When the download completes, close the window.

## Install Power BI Connector

You can install Power BI Connector by wizard or command line.

### Wizard installation

1. Open the Power BI Connector installation file then select **Yes** to confirm running the installation file.

1. Accept or change the temporary setup extraction folder and select **OK**.

    The **Power BI Connector Setup Wizard** opens.

1. Select **Next**.

1. (Optional) To install the connector to an on-premises data gateway, select **On-premises data gateway installation** and specify the custom data connector directory for your on-premises data gateway.

    For more information about on-premises data gateway installations, see the Microsoft documentation [Use custom data connectors with the on-premises data gateway](https://learn.microsoft.com/en-us/power-bi/connect-data/service-gateway-custom-connectors).

1. Select **Next**.

1. Select **Install**.

1. Select **Finish** to exit the Setup Wizard.

### Command line silent installation

To silently install Power BI Connector, open a command line session, change to the installation file download directory, and enter the following command:

```bash
.\AVEVA_Data_Hub_Power_BI_Connector_x_x_x_x.exe -Y INSTALLDIR="<install path>" /quiet
```

- Replace `x_x_x_x` with the version number of the installer.

- Power BI Connector supports silent installation for on-premises data gateway installations.

| Introduction |   |
|--------------|---|


The Application Administrator tool is just one part of a larger system called
the Mobile Application Platform. Note in the graphic below how the Motorola
Platform and Tools work together. You can use this secure and completely
integrated system to do the following:

-   The Application Server uses web services and communicates with the
    Application Administrator tool and the Motorola Adapter Designer. All
    metadata in the metadata database is available through the combination of
    the Application Administrator tool and the Motorola Adapter Designer. In
    addition, the Application Administrator tool is a browser-based application
    that provides you with data management and business object administration.
    Through a convenient user interface, you can create, edit, and delete a
    broad range of business object information; configure business rules and
    business constants; and manage messaging, conflict detection and resolution,
    performance, and troubleshooting.

-   Both the Adapter Designer and the Application Administrator tool employ
    intelligent-data adapters to manipulate data sources on servers.

-   The Motorola Application Designer enables you to configure, assemble,
    customize, and build new applications without writing a single line of code.
    This tool uses the Application Framework to develop applications bound to
    data definitions in metadata by abstracting the application from the data
    living in the back end enterprise application.

![Motorola Architecture](media/e94ba4cf80f4ebaec9e61aa94282e527.jpg)

### Identifying the Documentation Scope and Audience

The *Application Administrator tool Guide* provides information about using
Application Administrator tool to configure system-level administrator options
on the Motorola Application Server. System administrator tasks include
configuring data sources, security, and logging. This guide is intended for
system administrators who configure applications, data sources, security, and
logging using the Application Administrator tool.

#### Identifying References

The Mobile Application Platform documentation suite includes the following:

-   *Mobile Application Platform Installation Guide:* This guide provides
    information about installing the Mobile Application Platform.

-   *Application Server Configuration Guide:* This guide provides information
    about configuring the Motorola Application Server and metadata database.

-   *Mobile Application Platform Release Notes:* This guide provides information
    about various features and known issues in the Mobile Application Platform.
    It also provides the version number information of various Mobile
    Application Platform components.

-   *Adapter DesignerGuide:* This guide provides information about creating and
    editing Connections, Commands, Data Objects, and Views.

-   *Motorola Application Designer Guide:* This guide provides information about
    using the Motorola Application Designer to design forms for applications
    that are deployed to handheld devices, such as the Pocket PC (PPC), and used
    by field personnel.

-   *Deployment Manager Guide for PC:* This guide provides information about the
    procedures required to prepare a Dexterra Pocket PC application for mass
    distribution to field personnel.

-   *Dexterra Deployment Guide for Windows Devices:* This guide provides
    information about the procedures required to prepare a Motorola PDA
    application for mass distribution to field personnel.

-   *Dexterra Smart Client API Reference:* This guide provides information about
    how to write applications by using the constants and data types.

#### Defining Terms, Acronyms, and Abbreviations

The table contains some definitions of terms and acronyms that are used within
this guide.

| **Term**                                                 | **Definition**                                                                                                                                                                                                                                                                 |
|----------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SSL                                                      | Secure Socket Layer                                                                                                                                                                                                                                                            |
| Simple Object Access Protocol (SOAP)                     | SOAP is a protocol for exchanging XML based messages over a computer network. It enables messaging over HTTP on port 80 and uses a standard means of describing data.                                                                                                          |
| User Interface (UI)                                      | UI refers to the front end of the software, which provides a simple and easy to use interface between a computer and an application. An example is the Connection User Interface used to connect the adapter to the server.                                                    |
| Universal Description, Discovery, and Integration (UDDI) | UDDI enables organizations and individuals to publish information about themselves and the Web services they are offering. It is a global directory open to everybody, simple to use, and comprehensive in its scope.                                                          |
| Web Services                                             | A Web service is a collection of protocols and standards used for exchanging data between applications or systems. It provides a standardized way of integrating Web-based applications using the XML, SOAP, WSDL, and UDDI open standards over an Internet protocol backbone. |
| Web Service Description Language (WSDL)                  | WSDL describes the public interface to the Web Service. This is an XML based service description on how to communicate using the Web Service; namely the protocol bindings and message formats required to interact with the Web services listed in its directory.             |

### Identifying Installation Requirements

To install the Mobile Application Platform, you must have the following hardware
and software components.

#### Adhering to Hardware Requirements

-   Disk drive: 250 MB of free space

-   Memory: 1 GB of RAM

-   Internal/External Drives: a CD-ROM drive is required for program
    installation and access to the online documentation, which can optionally be
    downloaded to disk.

-   Display: a graphic color display

-   Keyboard: a specific keyboard compatible with selected installation locale
    may be required for national language support.

-   Pointing device: A 3-button mouse for usability reasons.

#### Adhering to Software Requirements

-   Operating system: Microsoft Windows XP or Microsoft Windows 2003

-   Database: Microsoft SQL Server 2000 (Service Pack 4) or SQL Server 2005

-   IIS 5.0 or IIS 6.0

-   Visual Studio .NET 2005

-   Microsoft Windows Mobile 5.0 for Pocket PC SDK and Microsoft Windows Mobile
    5.0 Smartphone SDK (for developing Smart Device Applications in the Motorola
    Application Designer)

-   Microsoft Data Access Components (MDAC), v2.7

-   .NET framework 1.1 and 2.0

-   Active Sync 4.1

#### Adhering to Software Requirements for Windows Server 2003

The software requirements for the Motorola Application Server for Windows 2003
are:

-   Windows Server 2003

-   Internet Information Server 5.0 (you must install IIS before installing the
    .NET Framework)

-   Microsoft Data Access Components (MDAC) v2.7

-   .NET Framework Distributable v1.1 and 2.0

-   Microsoft SQL Server 2000 (Service Pack 4) or Microsoft SQL Server 2005

#### Adhering to Software Requirements for Windows XP Server

The software requirements for the Motorola Application Server for Windows XP
are:

-   Windows XP Server

-   Internet Information Server 5.0 (you must install IIS before installing the
    .NET Framework)

-   Microsoft Data Access Components (MDAC) v2.7

-   .NET Framework Distributable v1.1 and 2.0

-   Microsoft SQL Server 2000 (Service Pack 4) or Microsoft SQL Server 2005

#### Adhering to Software Requirements for Windows Server 2003 Standard Edition

The software requirements for the Motorola Application Server for Windows 2003
SE (Standard Edition) are:

-   Windows Server 2003 Standard Edition

-   Internet Information Server 6.0 (you must install IIS before installing the
    .NET Framework. You must also install the ASP.NET and FrontPage 2003 Server
    Extensions options.)

-   Microsoft Data Access Components (MDAC) v2.7

-   .NET Framework Distributable v1.1 and 2.0

-   Microsoft SQL Server 2000 (Service Pack 4) or Microsoft SQL Server 2005

### Identifying Supported Devices

Motorola gives you the flexibility of writing applications targeting Windows®
5.0, Windows Mobile 2003 Second Edition, and Smartphone devices. As with any
platform, there are development considerations that must be taken into account.

For Windows Mobile 5.0 devices, you need to have their components and CAB files
signed if you write an application and rebuild the Deployment Manager CAB files,
This certificate issue is not limited to Dexterra components, but is an issue
for any components (including your own or other third parties') that are not
signed.

For Smartphones, the recommended software for Windows Mobile development is
Microsoft Visual Studio 2005. If you are using any other tools in addition to
Microsoft Visual Studio 2005, special care must be taken to install the
development tools in the correct order.

#### Using Windows 5.0 Pocket PC

The Motorola Application Designer fully supports the ability for application
developers to create smart applications on the new Windows Mobile 5.0 Pocket PC
(PPC) devices. A Windows Mobile device is a handheld device powered by the
Windows Mobile platform. It allows you to retrieve e-mail, track your schedule,
maintain your contacts, browse the Internet, and send or receive text messages.
Windows Mobile also allows you to download third-party software to customize
your device.

Businesses use Windows Mobile devices to help their employees communicate while
they are out of the office. The Windows Mobile platform is available on a
variety of devices from a variety of wireless operators. For more information on
Windows Mobile devices, see
<http://www.microsoft.com/windowsmobile/default.mspx>.

#### Windows 2003 Second Edition

Windows Mobile 2003 Second Edition is a handheld device that has a number of
improvements over Windows Mobile 2003. Besides being powered by the latest
Windows CE 4.21, other advancements include the support for Wi-Fi Protected
Access, an option in Pocket Internet Explorer (PIE) to scroll vertically by
forcing a page into a sing-column layout, and the support for a screen
resolution of 640×480.

Besides Pocket Word and Pocket Excel, other applications include, Pocket
Internet Explorer (PIE), Windows Media Player 9 Series for Pocket PC, and Pocket
MSN.

#### Using **Smartphones**

A Smartphone is a handheld device that combines the features of a mobile phone,
personal digital assistant (PDA), and handheld computer. This is something like
adding basic telephone functions to a PDA or adding PDA functions to a mobile
phone. You can also install additional applications, such as those built with
the Composer tool, on a Smartphone, on a Smartphone.

|                                          | [./media/image2.jpeg](./media/image2.jpeg) |
|                                          |                                            |
| Motorola Application Server Architecture |                                            |
|------------------------------------------|--------------------------------------------|


~   H2 logo

The Motorola Application Server is just one component of the overall Mobile
Application Platform and Tools enterprise architecture. This includes the
Application Administrator tool, the application database, the metadata database,
and the mobile applications that developers design. This is shown in the
following graphic.

![Motorola Server Architecture - 2](media/a30e2d199e168b02e0ba7e24759f4a5f.jpg)

The Motorola Application Server is a policy-driven engine that controls the
distribution of information and intelligently updates back end application
databases with changes that are made in the field by field personnel. The
architecture of the Motorola Application Server includes the following services
and components.

-   **Application Administrator tool:** This is a graphical user interface (GUI)
    used to configure the Motorola Application Server and Dexterra mobile
    applications.

-   **Metadata Database:** This is a data store that contains policy information
    about the business objects, business constants, and business rules related
    to applications deployed on the Motorola Application Server. For more
    information, see [Metadata Database](#metadata-database).

-   **Application Database:** This is a data store that holds the information
    related to the application.

-   **Mobile Application:** This is a Motorola Client Application that resides
    on a mobile device, such as a Pocket PC or a Tablet PC device.

### Understanding the Application Administrator tool

The administrative tasks described in this document are performed using the
Application Administrator tool. The Application Administrator tool is a GUI
front-end that works with the Motorola Application Server and is composed of
HTML and ASP.NET pages. As described in the *Dexterra Server Configuration
Guide*, an IIS Web server must be installed on the server on which the Motorola
Application Server is installed. This Web server hosts the HTML and ASP.NET
pages used by the Application Administrator tool.

### Application Administrator tool User Roles and Accounts

The options available in the Application Administrator tool may vary depending
on the security group to which your Application Administrator tool user account
is assigned. By default, there are three categories of security groups. They are
listed as follows:

-   Developers

-   Analysts

-   Administrators

Each security group is associated with a different set of privileges. These
privileges control the administrative options available to a user when they log
on to the Application Administrator tool. Administrative options appear on the
left side of the Application Administrator tool GUI as shown in the following
graphic.

![2_SecurityGroupAdministrativePrivileges](media/3cc3187ebfce8bd2450cde782e54faaf.jpg)

#### Logging on to the Application Administrator tool 

The administrator procedures described in this guide are performed using the
Application Administrator tool. The default path of the Motorola Application
Server is <http://localhost/DexterraServer/default.aspx>. When you log on to the
Application Administrator tool for the first time, the login service uses
localhost as the server by default. In case you enter a server name other than
localhost, the Application Administrator tool uses this server name when you log
on to the server the next time. You must enter a database name if you have
entered a server name. If you do not enter a value in the Server Name box, the
Server uses localhost as the default server and MASMetadata as the default
database.

##### T**o log on to the Application Administrator tool**

1.  Navigate to the default page of the Application Administrator tool:
    <http://localhost/DexterraConductor/Login.aspx>, where localhost is the name
    of the server on which the Motorola Application Server is installed. The
    Application Administrator tool Login page appears as shown in the following
    graphic.

![App_Admin_Login_Page](media/05551a474b5697534aa2540eaa0506bc.jpg)

1.  In the **Username** box, enter an administrator user name. The installer
    creates a default user that is part of the Administrators group. That
    default user name is **admin**. For information on changing the default
    administrator account credentials, see [Changing the Default Administrator
    Account
    Credentials](#changing-the-default-administrator-account-credentials).

2.  In the **Password** box, enter the password for the account. The default
    password is **password123**.

#### Changing the Default Administrator Account Credentials

Until changed, the default administrator account credentials are:

-   username: **admin**

-   password: **password123**

To ensure the security of your server, change the credentials for this account
as soon as possible.

##### To change the administrator account credentials

1.  Log on to Application Administrator tool as a member of the administrators
    group.

2.  Under the Security heading in the left pane, select **Users**.

3.  In the User ID column, click the **admin** user.

4.  If necessary, change the user name of the admin account by modifying the
    name in the **User ID** box.

5.  Click the **Change** button to change the admin password.

6.  In the **Old Password** box, enter the default password as **password123**.

7.  In the **New Password** box, enter the new password.

**Note:** The password is composed of letters and digits and cannot contain more
than 25 characters. Passwords cannot be left blank.

1.  Click the **Submit** button to save the changes. The password is changed,
    and you are returned to the User form.

2.  Be sure to add the user to the Administrator group as described in [Adding
    Users to a Group](#adding-users-to-groups).

### Identifying the Tasks of an Administrator, Developer, and Analyst 

As a system administrator, you typically perform the following tasks:

-   Define or change the security settings of the Motorola Application Server.
    By changing these settings, you affect how mobile users are authenticated
    and authorized for information.

-   Configure security groups to define custom administrative privileges.

-   Configure users associated with security groups.

-   Configure logging options.

-   Review logs.

-   Resolve any manual resolution record conflicts.

As a developer or analyst, you typically perform the following tasks.

-   Define applications and business objects (a data access layer for the client
    applications).

-   Define resources used in associating files in the server processes and in
    the client applications.

| Create and Modify Business Constants | [./media/image2.jpeg](./media/image2.jpeg) |
|--------------------------------------|--------------------------------------------|


~   H2 logo

Agile controls are found on the Dexterra Toolbox and allow you to bind data from
business objects to the controls. For example, you can bind Customer business
object data to an agile list view. As the Customer data is edited and updated in
the database, those updates are shown in the agile list view automatically once
the form that holds the list view is loaded.

The agile controls are a set of controls that inherit from the corresponding
versions of the standard Microsoft .Net framework controls, which are part of
the Microsoft Visual Studio software. Motorola has extended these controls by
adding BusinessObject binding functionality as well as miscellaneous other
properties. The Agile Control interface is the base interface for all other
agile control interfaces. This interface is used to bind the control to a
BusinessObjectSet component. It allows the business object set to direct the
population of the data on the control.

The AgileTenKey compound control is the only agile control that does *not* have
data binding capabilities. If you do not need properties on controls to change
with changing business object data, you can use the standard controls on the
Device Controls Toolbox that are included with the Microsoft Visual Studio
software. The following table contains a list of the Dexterra agile controls,
which are listed alphabetically.

| **Agile Control Name** | **Definition**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| AgileButton            | This custom control displays a standard button and binds the Text property to Business Object properties.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| AgileCheckBox          | This custom control displays a standard check box and binds the Checked property to a Business Object property.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| AgileComboBox          | This custom control displays a standard combo box control and binds the SelectedValue property to a BusinessObject property. The list for the combo box is then bound to a business object set. In a design scenario in which two agile combo boxes are in a master/child relationship, for example, and each is bound to a separate business object set, make sure to set properties so that the child combo box either gets its information from the business object set *or* the master combo box. Otherwise, an exception occurs at run-time. **Note:** Do not set actions to the Click event for an AgileComboBox. The Click event does not fire. This is due to Microsoft .NET functionality in the Combo box.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| AgileDateTimePicker    | This custom control is similar to the DateTimePicker control in the full version of the Microsoft .Net framework. The Dexterra control behavior is derived from the .NET behavior. **Available :** 1/1/1752- 12/31/9998.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| AgileLabel             | This custom control displays a standard label control and binds the Text property to a BusinessObject property.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| AgileLinkLabel         | This custom control displays underlined text. It binds the Text property to a BusinessObject property.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| AgileListBox           | This custom control displays a standard list box control and binds the SelectedValue property to a BusinessObject property. The list for the list box is also bound to a business object set.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| AgileListView          | This custom control displays a standard list view control and binds it to a business object set. The KeyProperty is used to reselect the item in the ListView. It doesn't necessarily have to be unique.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| AgileMenuItem          | This custom component displays a standard menu item control and binds its Text property to a BusinessObject property. Once it has been added to a form, you can add a SubMenuItem (also known as a menu option).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| AgilePageView          | This control provides paged access to business object data. It is similar to the AgileListView control in that it allows end users to see business object data. It also has additional functionality to manage contents by employing Back and Next navigation through the pages. Note that the number of rows in an agile page view decreases by one when the ImageColumn property is set to True and ImageList property is set to any ImageList object. This is because the default image size in an ImageList property is 16x16. The row height must be increased to accommodate the image height. This results in fewer visible rows, because the overall height of the control doesn't change. Also note that the Size property or the height of the control is calculated by a combination of the visible rows and the size of the selected font.                                                                                                                                                                                                                                                                                                                                                                                         |
| AgilePictureButton     | This custom control displays a standard picture box control and binds the Image property to a BusinessObject property. The BusinessObject property values must be binary data that holds images.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| AgileRadioButton       | This custom control displays a standard radio button and binds the Checked property to a BusinessObject property.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| AgileSignature         | This custom control displays a standard panel control with a black border around the edge. You can employ it to capture the vector coordinates as you drag the stylus around the client surface of the control. It binds the coordinate string to a BusinessObject property of type string.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| AgileTextBox           | If the control is edit-enabled (meaning the Read-Only property is set to False), the Text property is bound to the single editable BusinessObject property specified in the EditProperty property. If the control is not edit-enabled (meaning the Read-Only property is set to True), the Text property is bound to the BusinessObject properties specified in the DisplayProperties array. For the FontName property of the AgileTextbox, make sure to use fonts that are supported by Microsoft .NET Compact Framework. **Note:** The TextChanged event of the AgileTextBox is fired when the text within the box changes. This is standard Microsoft .NET behavior. To avoid this, you can use an ActionNotify action and an ActionGetSet action. Tie the ActionNotify Succeeded event to the ActionGetSet action. Also note that the AgileTextBox returns *Type* instead of *Value* when used in conjunction with the ActionGetSet action. This is Microsoft .NET Compact Framework behavior. The Dexterra Composer Framework derives its behavior from the Microsoft .NET Compact Framework. You can get another value other than Type name by overriding the ToString method on the object that is being converted by the ActionGetSet. |
| AgileToolBarButton     | This custom control displays a standard toolbar button. The Image property of the button can be bound to a BusinessObject property. The toolbar that contains this toolbar button is automatically included in the frame that contains forms during run-time.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| AgileTreeView          | This custom control displays a standard tree view control and binds its nodes collection to a BusinessObjectSet component. If a tree descriptor is not bound to a **LinkProperty**, it displays all immediate business objects in the business object set. If a tree descriptor is bound to a **LinkProperty**, it displays all business objects in the BuisneesObjectLink for the business object set's CurrentBusinessObject. Since the agile tree view control is not a Set control, it does not set the CurrentBusinessObject when the user selects a node.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

#### Defining the AgileTenKey Compound Control

This is a compound control that contains ten buttons, which represent each of
the ten numeric digits. It is the only agile control that does *not* bind to
business object data. When an end user clicks any of the buttons, the
corresponding digit is added to the control’s Text value.

![tenKey](media/05c9d5991c326090b0b0b3d3d92a70e3.jpg)

#### Defining the Edit Property

The Edit property determines the name of the Business Property to which the
agile control is bound and is allowed to edit.

#### Defining the AutoPersist Property

The AutoPersist property determines if changes to the underlying Business
property – to which the agile control is bound – should also be carried over to
the agile control. If this property is set to True, the control’s value is
carried over to the underlying Business Property until once the focus is no
longer on that control.

### Binding the Data to the Agile Controls

Data binding happens through the use of agile controls. You can bind a business
object set to an agile list view for example. When information is changed within
the business object set, the change is automatically reflected in the list view
when the form that holds the list is loaded. In order to accomplish this, you
must access metadata on the server when you first set the properties of agile
controls.

|                                 | [./media/image2.jpeg](./media/image2.jpeg) |
| Business Objects Configuration  |                                            |
|---------------------------------|--------------------------------------------|


~   H2 logo

Business objects are a very prominent part of the Motorola Application Designer
and its components. To develop flawless applications, one must have an
exhaustive knowledge of business objects, creating it, and understanding the
various events associated with it.

### Understanding Business Objects

A Dexterra business object represents a specific type of data used by the
Dexterra application. Examples include product, product number, appointment, and
so forth. Business objects defined and modified using Application Administrator
tool are physically stored in the metadata repository.

The Dexterra version of a business object packages data source metadata that is
passed to the device and then manipulated by your small factor application’s
public class BusinessObject statement(s). Unlike the BusinessObject class,
however, a Dexterra business object does not contain any business logic. The
business logic is completely contained in your Visual Basic code.

The Dexterra metadata repository contains the schema for the business objects,
business rules, business constants, views, and columns used by the Motorola
Application Server. The metadata repository is stored in a SQL Server database.
When the Pocket PC user selects the Motorola Settings, Subscribe tab, and Get
Customer Data Definition option, the metadata b_mac database is created and
populated with data from the metadata repository. Any defined Dexterra business
objects are used to create the b_mac table definitions. The following graphic
illustrates the relationship between Dexterra business objects and Dexterra
views, and between Dexterra business object properties and Dexterra view
columns.

![ServerPropertyDiagram](media/07545e5fbcd8121ba32523e3a51a4d07.jpg)

#### Defining Business Objects

Because of the relationship between fields and tables in the application
database and the business objects defined in the metadata repository, database
administrators typically define business objects.

##### To create a business object 

1.  Start the Application Administrator tool.

2.  From the Business Information category in the left pane, select Business
    Objects.

3.  In the Business Object box, enter a unique name of your new business object.
    This name is referenced by your Dexterra Field Service.

4.  Enter a description for this new business object. The Business Object box
    should look similar to the one shown in the next graphic.

![BusinessObjectProjectWindow](media/993e75869977e243c9e8f697d2378f11.jpg)

1.  Click the Save icon to save your new business object.

2.  Click the Views tab to display the Views in Business Object form.

3.  From the Views in Business Objects list, select the view (client table) that
    you use to populate your business object.

![](media/1c3bd3b532b40c5a0097cbf5129034a7.png)

1.  Repeat the previous step to add as many views as required to populate this
    business object. These subsequent view/client tables may contain pertinent
    foreign key columns.

![ViewsinBusinessObjectWindow2](media/96d151374be888832adfba7b9ff3b385.jpg)

1.  For each view/client table, specify a unique client table alias. This alias
    is used in any FROM and/or WHERE clause that you define.

2.  In the Update column, click the Update button for the table that need to be
    updated when you save the business object. Only one table can be marked as
    updatable on the device.

3.  In the Where Clause box of the From & Where section, enter the appropriate
    WHERE Transact-SQL to determine the condition(s) under which the specified
    client table view rows should be returned. This WHERE clause is started on
    the Pocket PC device, not on the server.

Here is an example of a WHERE clause:

For the client tables, a_SelectionType (with the alias a_selection and the
primary key k_selection) and a_product (with the alias a_product and the foreign
key k_selection):

a_product.k_selection = a_selection.k_selection

By default, the device automatically generates a FROM clause using the following
format:

client_table_name as client_table_alias[, ...client_table_name as
client_table_alias]

for example,

a_actionitem as a_actionitem_1, a_selection as a_selection_1, a_selection as
a_selection_2

It is important to note that this FROM clause does not include any JOIN
statements.

To override this auto-generated FROM clause and provide a different FROM clause,
(perhaps including a JOIN or OUTER variant), select the Override FROM Clause
box. The From Clause box becomes available.

In the From Clause box, enter your alternate FROM Clause, being sure to
reference the client table view alias instead of the table name.

**Note:** Do not include the FROM keyword when specifying a FROM clause using
the Application Administrator tool. The Application Administrator tool includes
the FROM keyword in the generated SQL.

Here is an example FROM clause:

For the client tables a_selection (with the aliases a_selection, a_selection_1,
and a_selection_2 and the primary key k_selection) and a_actionitem (with the
alias a_actionitem and foreign keys ks_actionitem, ks_priority, and ks_billing):

a_actionitem join a_selection on a_actionitem.ks_actionitem =
a_selection.k_selection join a_selection as a_selection_1 on
a_actionitem.ks_priority = a_selection_1.k_selection left outer join a_selection
as a_selection_2 on a_actionitem.ks_billing = a_selection_2.k_selection

This is how the above FROM clause appears in the Conductor tool window:

![](media/17dcfe8affc9b555f10891714192acdf.png)

1.  To override all of the Motorola Application Server auto-generated WHERE and
    FROM SQL statements for the selected business object (effectively making the
    business object read-only), clear the Override From Clause box and select
    the SQL Pass-Thru box.

In the following example, first a property named PassThru is created. Then the
property is passed as a variable using the WHERE statement.

In this example, a property is created and then assigned to an unused column.
Once the property is created, the name of the property alias is appended with
\~\~ to indicate that it is a variable. Another example could include:

select ai.k_issue

from a_actionitem ai,a_entity apuser

where ai.k_user = \~\~apuser.k_entity\~\~

It is very important to note that you must reference the correct columns and
alias names.

![BusinessObjectCustomerWindow](media/510120061673c7ba52cc509698d3d8d8.jpg)

#### Removing a Client Table View from a Dexterra Business Object

If you remove a client table from a Dexterra business object, always remember to
scan the associated WHERE and FROM clauses and remove any references to that
client table.

##### To remove a client table view from a business object 

1.  Start the Application Administrator tool.

2.  From the Business Information category in the left pane, select Business
    Objects.

3.  In the **Business Objects** list, click the name of the business object
    containing the client table view you want to remove.

4.  Click the **Views** tab.

5.  In the Views in Business Object page, locate the name of the client table
    view you want to remove from the business object definition and click
    Remove.

**Note:** If the client table view you just removed is referenced in either, the
user-specified WHERE or FROM clause, be sure to edit these as necessary.

1.  Click the Save icon.

##### To delete a Dexterra business object

1.  Start the Application Administrator tool.

2.  From the Business Information category in the left pane, select Business
    Objects.

3.  In the Business Objects list, locate the business object you want to delete.

4.  Click the **associated Delete** link.

5.  Click the **Save** icon.

#### Defining Business Object Properties and Mapping them to Business Object Columns

The business object defines the dataset that would be available to the business
object. Business object properties enable you to refer to the columns returned
by the views. These properties can be referenced in your custom code using the
Property Alias you define in Application Administrator tool.

#### Working with the Alias Business Objects for Better Performance

The Application Administrator tool provides a way to duplicate business object
properties across your business objects by using one property definition for
multiple business object properties with a property alias. See the example
illustrated in the following graphic:

![PropertyNamePropertyAliasWindow](media/982177e4ce58fa6a3ade7393085b3d65.jpg)

#### Understanding the Business Object Links

One of the properties of a business object is that, it can be a referenced to
another business object or objects. Take, for example, a Customer business
object and a Customer Address business object. By linking Customer and Customer
Address, you can efficiently retrieve the array of addresses associated with a
particular customer.

#### Saving Related Objects (Children) When Saving the Business Object

When a complex property is referenced in a business object link, the client
implicitly queries for the related objects. Also, if changes are made to the
business object, any save or delete actions to the business object are
propagated to its related objects if explicitly specified in the code.

#### Understanding the Foreign Keys

A foreign database key is a key that references, or targets, a key (usually a
primary key) in a different table.

#### Understanding the One-to-One and One-to-Many Table Column to Table Column Relationships

A one-to-many relationship exists when only one of the related columns in a
table is a primary key or has a unique constraint. An example of a one-to-many
relationship would be a table containing customers and another containing
customer phone numbers. Each customer can have multiple associated phone numbers
(work, cellular, fax, and so forth). The customer table can have many matching
rows in the phone numbers table, but a row in the phone number table can have
only one matching row in the customer table.

A one-to-one relationship is uncommon and not widely known. It exists if both of
the related columns (in separate tables) are primary keys or have unique
constraints.

##### To create a Dexterra business object property

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Properties**.

3.  In the Name box, enter a unique name for this business object property.

4.  (Optional) In the **Default Value** box, enter the default value for this
    Dexterra business object property. If you are defining a business object
    link, ignore any value entered in this box.

5.  (Optional) In the **Minimum Value** box, enter the minimum value for this
    Dexterra business object property. If the property you are defining is a
    String data type, then minimum value refers to the minimum length of the
    string. If the property you are defining is a numeric data type or a date or
    time data type, then this refers to the minimum value of the property. If
    you are defining a business object link, ignore any value entered in this
    box.

6.  In the **Maximum Value** box, enter the maximum value for this Dexterra
    business object property. If the property you are defining is a String data
    type, then maximum value refers to the maximum length of the string. If the
    property you are defining is a numeric data type or a date or time data
    type, then this refers to the maximum value of the property. If you are
    defining a business object link, ignore any value entered in this box.

![PropertyWindow](media/2d4225585dadbc82d9c93158a22c5f1c.jpg)

1.  In the Data Type box, choose from one of the pre-defined data types.

2.  If you select the data type Business Object Link in the Data Type list, the
    Business Object Link list is populated with already defined Dexterra
    business objects. Choose one Dexterra business object to which you need to
    link this property.

If you select a business object from the Business Object Link list, the Business
Object Property list is populated with already defined properties of that
business object. Choose one property (usually a primary or foreign key) to which
this property need to be linked.

**Note:** This list is available only if you have selected a business object
link in the Business Object Link box.

1.  If you want this property to contain an array of values, select the Array
    check box.

2.  Click the **Save** icon.

**Note:** The Business Objects using Property tab displays a list of all of the
Dexterra business objects you previously defined that use this property. The
information on this tab is read-only. To alter a business object or business
object property definition, click either **Business Objects** or **Properties**
in the left panel.

##### To map a Dexterra business object property to a view column

Use this procedure to create a relationship between a business object and a
business object property or business object link property.

**Note:** The Dexterra business object and property name to which you want to
map a view column must have been previously defined.

1.  Start the Application Administrator tool.

2.  From the Business Information category in the left pane, select Business
    Objects.

3.  Choose the appropriate business object from the Business Objects section.

4.  Click the Properties tab.

5.  In the Properties of Business Object list, choose the name of the already
    defined property that you want to map to a data source view column. Only
    properties from the business object named in step 3 are displayed.

6.  (Optional) To map more than one instance of a particular property to more
    than one view column, enter the number of property instances you want to
    create in the numeric box to the right of the Properties of Business Object
    list.

7.  Click the Add link.

This appends a new row is to the Properties of Business Object list and the
business object property you selected is displayed in the Property Name column.

##### To delete an existing business object property

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Properties**.

3.  In the **Properties** list, locate the property you want to delete.

4.  Click the associated **Delete** link.

##### To delete a business object

1.  Start the Application Administrator tool.

2.  From the Business Information category in the left pane, select Business
    Objects.

3.  In the Business Objects list, locate the business object you want to delete.

4.  Click the Delete check box to the left of that business object.

5.  Click the OK button.

### Using Resources

Resources are Dexterra’s way of identifying files that must be included as part
of the Dexterra system. A resource can represent a .txt, .dll, or an .exe file.
The files used by the system either on the server or on the client are also
included. In this section, we are referring to a resource that is used in the
Motorola Client Application for validating/manipulating business object data.
These resources are the class libraries compiled in a .dll.

#### Creating a Business Rule Resource

In Visual Studio, you create your Business Rule as a class. You have to compile
your Business Rule class into a DLL. This is needed for the platform on which it
is deployed.

#### Naming your Assembly in the Application Administrator tool

To call a business rule from a business object event, and to configure the rule
in the Administrator, you need to refer to its DLL class.

##### To name an assembly in the Application Administrator tool 

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Assemblies**.

3.  In the **Name** box, enter a descriptive name for your assembly. This name
    must be unique.

4.  Fill in a Version and Revision number. This is use to keep track of the
    current version so that a newer version can be recognized and deployed to
    the client.

5.  Select the **Required Resource** box indicating that this file is required
    for the Motorola Client Application to run.

6.  Clear the **Execute after download** onto device. This is used for deploying
    .CAB installation files or an executable that needs to start once it is
    deployed to the device.

7.  In the **File to Save** box, enter, or locate the DLL that you want to load
    into the database. The actual filename is derived from the path and
    displayed in the read-only **File Name** box.

8.  Leave the **Install Path Override** box blank. This determines the path in
    which this file should be copied to the client device. Typically, your
    Business Rule DLL needs to be in the same directory as your application.

9.  Leave **Command Line** blank.

10. Select the right platform. This is used since it is possible that an
    Application has a Pocket PC version AND a laptop version. In this case, you
    would only want the Pocket PC based DLL on the PDA and the windows based DLL
    on the laptop.

11. Click the **Save** icon.

#### Adding a New Business Object to your Small Factor Application

After you have defined a business object, you must check if it is available in
your application. When your Get Application Definition code is started (during
the subscribe procedure, for example), the metadata that describes your business
object is downloaded into the m_mac.sdf database on the Pocket PC. Before your
business object can be accessed on the Pocket PC, it must be added to the
application.

##### To add a new business object to an application

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Business Objects**.

3.  Click the business object you want to add to the application.

4.  From the **Applications using Business Object** list, choose an application,
    and click the **Add** hyperlink.

5.  Click the **Save** icon.

##### To remove a business object from an application

1.  From the **Business Information** category in the left pane, select
    **Business Objects**.

2.  Click the business object you want to remove from your application.

3.  In the Applications using Business Object table, click the **Remove**
    hyperlink.

4.  Click the **Save** icon.

| Business Rules and Constants  | [./media/image2.jpeg](./media/image2.jpeg) |
|-------------------------------|--------------------------------------------|


~   H2 logo

Business rules enable you to apply consistent logic to your business data. In
general, business rules define:

-   **How data is handled when it is manipulated** (inserted, updated, saved,
    reverted, located, or deleted)**:** Take, for example, a business rule that,
    on a save action, checks a service estimate against the contact of the
    customer monetary authorization limit. This type of business rule is
    triggered by a business object event—an event that is associated with a
    business objects using the Application Administrator tool.

-   **How data is handled when it is validated:** Take, for example, a business
    rule that verifies that there are nine digits in a social security number or
    that a company has required identification code has been entered.

-   **How data integrity is handled:** For primary keys of type String, for
    example, your business rule can ensure that the key remains unique.

Business rules enable the functionality defined in your .NET source code. For
example, the JobTitleRequired business constant can be set to True or False.
However, the logic that actually checks to verify whether a Job Title must be
provided and what happens if the job title is not provided is enabled by a
business rule. In this case, an event triggers the business rule, and then
business constant, to be evaluated. Use the Application Administrator tool to
specify the business rule that would be started either before or after any of
the above events.

**Note:** The logic used to enable a business rule is defined in a DLL, which is
developed using VB.NET. The Application Administrator tool is used to define the
business rule by referencing the business rule DLL.

**Note:** Business rule definition information is stored in the metadata
database.

### Invoking Business Rules

On the device, a business rule is invoked by your custom code or by a business
object event. On the server, a business rule is invoked by an event generator.

### Defining Business Rules 

Because business rules use DLLs to enforce rules, business rules are typically
created by database administrators or developers using VB.NET.

### Creating Business Rules

There are two general steps to creating a business rule for use by your small
factor application. These are:

-   Use Microsoft Visual Studio to create a business rule class. Add Evaluate
    and TakeAction code. Compile this into a DLL.

-   Using the Application Administrator tool, name the data manipulation event
    that trigger the business rule.

Or you can create an event generator that fires the business rule at a specific
time or time interval. For more information, see [Defining Event
Generators](##_Defining_Event_Generators).

### Using Microsoft Visual Studio.NET to Create a Business Rule

Before mapping to a business rule using the Application Administrator tool, you
must have already created the business rule class in Microsoft Visual Studio. An
example of an address validation business rule is shown in the next graphic.

![BusinessRulesWindow](media/ed96ac069690fc3285b4f1e7dfe576b2.jpg)

The AddressValidate business rule shown in the graphic above and in the code
following, for example, identifies each required input box and the action to
take if the user does not enter a value. In each case, a message (a business
constant) is displayed.

In the first line, AddressValidate refers to the Business Rule. This is
referenced in the Application Administrator tool as
Dexterra.Apps.BusinessRules.AddressValidate (the full namespace of the class
file). The second line is necessary, as your business rules must always inherit
from BusinessModel.BusinessRule.

Public Class AddressValidate

Inherits BusinessModel.BusinessRule

### Defining Business Rules in the Application Administrator tool

After creating a business rule code in Microsoft Visual Studio, you need to
define the business rule in Application Administrator tool.

##### To define a Dexterra business rule

1.  Start the Application Administrator tool.

2.  From the Business Rules category in the left pane, select **Business
    Rules**.

3.  In the **Class Name** box, enter a unique class name identifier for this
    business rule.

4.  Select the assembly from the **Assembly** list to which you want to link the
    class you named in step 3.

**Note:** Usually, the assembly linked to a business rule contains DLLs that, in
turn, contain the actual compiled business rules.

1.  Click the **Save** icon.

![BusinessRulesRecordsWindow](media/9084320e145b5f6c7795f484f2337e07.jpg)

1.  To view the event generators using the selected business rule, select the
    **Event Generators** tab. The information displayed on the Event Generators
    tab is read-only. For more information, see [Defining Event
    Generators](##_Defining_Event_Generators).

2.  To view any business objects associated with this business rule, select the
    **Business Objects** tab. The information displayed on the Business Objects
    tab is read-only. For more information, see [To define a Dexterra business
    object event and map it to a business
    rule](#to-define-a-dexterra-business-object-event-and-map-it-to-a-business-rule).

### Analyzing Business Categories and Constants

Business constants are globally available strings that can be used for
application-wide business rules.

**Note:** With this release, it is possible to replace the value of a
server-side business constant with a value from a client device. For more
information, see [Synchronizing Client Variables and Business
Constants](#synchronizing-client-variables-and-business-constants).

Business categories enable you to classify your business constants. Usually, you
create a business category for each distinct business rule. Using the
Application Administrator tool, you can view, add to, and edit all of the
business constants associated with a particular business category/business rule.

#### Defining Business Categories

Before you can define business constants, you must define the category to which
it belongs.

##### To define a Dexterra business category

1.  From the Business Rules category in the left pane, select **Business
    Categories**.

2.  In the **Name** box, enter a unique name identifier for this business
    category.

3.  In the **Description** box, enter text describing the business constants
    that needs to be included in this business category.

4.  Click the **Save** icon.

5.  To view any business constant associated with a business category, and the
    order in which would appear if used as a list, select the **Business
    Constants** tab. The information displayed on the Business Constants tab is
    read-only. For information, see [To define a Dexterra business
    constant](##_To_define_a_Dexterra business const).

#### Understanding Business Constants

Business constants provide the values that can be used in a business rule. The
value of a business constant can be literal, Boolean, or literal with an
embedded temporary SQL variable as illustrated by the GetLatestWarningMessage
example in the table below.

| **Business Constant**   | **Value**                                                                                                                   | **Business Category:** |
|-------------------------|-----------------------------------------------------------------------------------------------------------------------------|------------------------|
| Address1Required        | True                                                                                                                        | AddressValidation      |
| Address2Required        | False                                                                                                                       | AddressValidation      |
| DefaultCountry          |                                                                                                                             | Defaults               |
| GetLatestWarning        | 8                                                                                                                           | Defaults               |
| GetLatestWarningMessage | It has been more than \~\~GetLatestHours hour(s) since inventory was updated. Product availability status may be incorrect. | Defaults               |
| ZipCodeFormatMessage    | Enter a five-digit or extended Zip+four Zip Code.                                                                           | AddressValidation      |
| ZipCodeRequired         | True                                                                                                                        | AddressValidation      |
| ZipCodeRequiredMessage  | Please supply a Zip Code.                                                                                                   | AddressValidation      |

In the GetLatestWarningMessage example, your SQL code would create a temporary
variable called \~GetLatestHours. Note that in the actual warning message, the
meta-tilde (two tildes) must be used to indicate that one tilde should be
retained.

##### To define a Dexterra business constant 

1.  From the Business Rules category in the left pane, select **Business
    Constants**.

2.  In the **Name** box, enter a unique name identifier for this business
    constant.

3.  In the **Value** box, enter the default value of this new business constant.
    Do not include the usual quotation marks required by Visual Basic unless the
    constant should include literal quotation marks. Examples include:

-   True

-   False

1.  Enter the customer’s First Name.

2.  If your constants are displayed as a list, in the **Order** box, enter a
    number to indicate this precedence of the constant in the list. Constants
    are ordered lowest order number to highest order number.

3.  From the **Category** list, select the business category to which this
    business constant would belong.

4.  In the **Description** box, enter text describing the business constant.

![BusinessConstantsWindow](media/85f900cdb0f3dad248a1ee681fea9c85.jpg)

1.  Click the **Save** icon.

### Synchronizing Client Variables and Business Constants

The Dexterra synchronization methods on the client enable you to replace the
value of a Motorola Application Server business constant with a value from a
client-side variable. With this functionality, you can pass a variable from the
Motorola Client Application to the Motorola Application Server. You can use that
variable value to customize the filter and, ultimately view the data downloaded
to the client. For example, you can view all of a person’s assigned work
tickets.

#### Using the SynchronizeApplication Method to Replace a Business Constant Value with a Client Variable

The following is the syntax for the SynchronizeApplication method:

Dexterra.Client.DefaultSyncUI.Sync.**SynchronizeApplication**

(*sApp* As String, deleteFromDataStore As Boolean, varNames() As String,
varValues() As String)

As Dexterra.Client.BusinessModel.BusinessConnector.eSync as listed below.

| **Parameter**       | **Description**                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| App                 | This is the metadata name of the application to synchronize.                                                                                                                                                                                                                                                                                                                                |
| deleteFromDataStore | A Boolean value that can be set to True if you want any process to be reflected on the client device data store. If deleteFromDataStore is set to False, process deletes would not be deleted on the client device data store. If, for example, a client variable changes a filter, you can delete records on the device that no longer match the filter by setting this parameter to True. |
| varNames            | A string array containing all of the variable names you want to pass. Variable names should be the same as the corresponding business constant names.                                                                                                                                                                                                                                       |
| varValues           | A string array containing the values for the variables you want to pass. These values must refer to a fully qualified constant in the form \<constant category\>.\<constant name\>.                                                                                                                                                                                                         |

For example:

Private Sub btnUpImage_Click (ByVal sender As System.Object,

ByVal e As System.EventArgs) Handles btnUpImage.Click

Dim varNames As String() = {"MyCategory.Constant1, MyCategory.Constant2"}

Dim varValues As String() = {"Dexterra", "True"}

Dim eRetVal As BusinessModel.BusinessConnector.eSync

‘to synchronize the entire Box Service Application

eRetVal DefaultSyncUI.Sync.SynchronizeApplication

End Sub

#### Updating a Single Business Object

Another new method, SynchronizeBusinessObject, enables the client to send a
single business object to the Motorola Application Server for updating.

#### Using the SynchronizeBusinessObject Method

The following is the syntax for the SynchronizeBusinessObject method:

Dexterra.Client.DefaultSyncUI.Sync.SynchronizeBusinessObject

(sApp As String,

sBO As String )

Dexterra.Client.DefaultSyncUI.Sync.SynchronizeBusinessObject (sApp As String,
sBO As String, deleteFromDataStore As Boolean, varNames() As String, varNames()
As String)

**Note:** The second overloaded SynchronizeBusinessObject method syntax can also
be used to pass client variables.

| **Parameter**       | **Description**                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| App                 | This is the metadata name of the application to synchronize.                                                                                                                                                                                                                                                                                                                                |
| sBO                 | String that specifies the business object you want to update.                                                                                                                                                                                                                                                                                                                               |
| deleteFromDataStore | A Boolean value that can be set to True if you want any process to be reflected on the client device data store. If deleteFromDataStore is set to False, process deletes would not be deleted on the client device data store. If, for example, a client variable changes a filter, you can delete records on the device that no longer match the filter by setting this parameter to True. |
| varNames            | A string array containing all of the variable names you want to pass. Variable names should be the same as the corresponding business constant names.                                                                                                                                                                                                                                       |
| varValues           | A string array containing the values for the variables you want to pass. These values must refer to a fully qualified constant in the form \<constant category\>.\<constant name\>.                                                                                                                                                                                                         |

For example:

Private Sub btnUpImage_Click(ByVal sender As System.Object,

ByVal e As System.EventArgs) Handles btnUpImage.Click

Dim varNames As String() = {"MyCategory.Constant1, MyCategory.Constant2"}

Dim varValues As String() = {"Dexterra", "True"}

Dim eRetVal As BusinessModel.BusinessConnector.eSync

End Sub

### Initiating the Business Object Events

An event either occurs before or after the user initiates any of the following:

-   Insert action

-   Update action

-   Save action

-   Revert action

-   Findset action

-   Find action

-   Delete action

Such actions, when appropriate, can be mapped to a business rule. So whenever
the event occurs, the business rule is triggered.

##### To define a Dexterra business object event and map it to a business rule

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Business Objects**.

3.  In the Business Objects list, locate and click the business object for which
    you want to define events.

4.  Click the **Events** tab.

5.  Click the **Add** box to the left of the appropriate event.

6.  Select the appropriate business rule from the Business Rule list, as shown
    in the following graphic.

![BusinessObjectAddress](media/0fbd4c9ae572c0dee9df241101f8af3c.jpg)

1.  Click the **Save** icon.

##### To remove a business object event definition

1.  Start the Application Administrator tool.

2.  From the **Business Information** category in the left pane, select
    **Business Objects**.

3.  In the Business Objects list, locate and click the business object from
    which you want to remove an event.

4.  Click the **Events** tab.

5.  Clear the **Add** box to the left of the appropriate event.

6.  Click the **Save** icon.

### Working with Event Generators

For business rules triggered by user actions, you associate an event with the
business rule as described in the section [To define a Dexterra business object
event and map it to a business
rule](#to-define-a-dexterra-business-object-event-and-map-it-to-a-business-rule).
There are occasions, however, when you want to fire a business rule at a
specific date and time or at specific time intervals. This is independent of
user actions. The following are some examples of date-based triggers for which
you may want to define an event generator.

-   Fiscal-year end

-   Loan Due

-   Bill Payable

#### Defining Event Generators

For business rules that should be fired at a specific date and time or a
specific time interval, you need to define an event generator and then tie that
event generator to your business rule.

##### To define an event generator

1.  Start the Application Administrator tool.

2.  From the **Business Rules** category in the left pane, select **Event
    Generators**.

3.  In the **Name** box, enter a unique name for this new event generator.

4.  Do one of the following:

-   If this is a one-time event select the **month, day, year, and military
    hours and minutes** time at which this event should be started in the
    Schedule Time list,. (Both date and time is initialized to the current date
    and time at which you selected the Event Generators link in the left
    navigation panel.) Then select the **Disable Schedule Time** box.

-   If this is a recurring event select the **month, day, year, and military
    hours and minutes** time at which this event should be initiated in the
    Schedule Time list,. (Both date and time is initialized to the current date
    and time at which you selected the Event Generators link in the left
    navigation panel.) Clear the **Disable Schedule Time** box. In the Interval
    (Sec) box, enter the number of seconds that should elapse between the start
    of this event and the next time it is started.

**Note:** The read-only Last Executed box displays the last date and time at
which this event was triggered.

1.  In the Business Rules tab, Business Rules of Event Generator list, select a
    business rule that triggers the event generator you just defined.

2.  Click the **Save** icon.

|                   | [./media/image2.jpeg](./media/image2.jpeg) |
| Metadata Database |                                            |
|-------------------|--------------------------------------------|


~   H2 logo

The metadata database stores policy information about the business objects,
business constants, and business rules that are related to applications and are
deployed on the Motorola Application Server. The metadata database is stored in
a Microsoft® SQL Server database, which is named *MASMetadata* by default. For
more information, see [Logging on to the Application Administrator
tool](#logging-on-to-the-application-administrator-tool) .

Unlike an application database, the metadata database does not store information
related to a specific application, such as part IDs, product names, or customer
information. Instead, the information in the metadata database is used to
configure the business policies that control the distribution of information.
This information is used to track which data is on which device. The server can
then determine what changes in data need to be sent to the client during a
synchronization process. In addition, the metadata database stores information
for application databases in the m_datasource table, as shown in the following
graphic.

![Metadata Database - 2](media/fd291df143a30a6c16c40b2303791bd4.jpg)

The metadata database can store information for multiple applications. For
example, the metadata database can contain connection information for an
enterprise application located in PeopleSoft and Oracle. The configuration
information for both of these applications can also be stored in the metadata
database, along with the business rules, business objects, and business
constants. This data can be used across all applications and is defined in the
metadata database.

#### Deploying the Motorola Application Server 

The Motorola Application Server can be deployed on a single server or across
multiple servers. However, regardless of the deployment approach, each Motorola
Application Server must be configured to use a single metadata database. For
single-server deployments, see [Connecting to a Local Metadata
Database](#connecting-to-a-local-metadata-database).

When a farm of Motorola Application Servers is deployed to handle sites with
high traffic volumes, each server in the farm must be configured to use the same
metadata database, as shown in the next graphic.

![Dexterra Server Deployment Strategies - 2](media/ba3a3aa3a2d3ecb3528725577cea7972.jpg)

You can find information about deploying the metadata database remotely on a
server that does not host the Motorola Application Server in [Connecting to a
Remote Metadata Database](#connecting-to-a-remote-metadata-database). The
metadata database is set up during the installation of the Motorola Application
Server using scripts that lay down the schema for the database. For more
information, see the *Dexterra Server Configuration Guide*.

**Note:** If the Requested registry access is not allowed error message appears,
you may have failed to grant the ASPNET user permission in the registry. See the
Verifying User Permissions section in the *Dexterra Server Configuration Guide*
to determine whether the correct ASPNET user permissions are in effect.

#### Identifying the Metadata Database Naming Conventions

By default, the metadata database is named *MASMetadata*. The name is assigned
to the database when you create the database using the installation scripts. For
more information about building the metadata database, see the *Dexterra Server
Configuration Guide*.

At times, you may choose to change the name of the metadata database. This may
happen in cases when you have a development, staging, and production environment
where you might have a unique metadata database for each particular environment.
Using a separate metadata database for each environment ensures that a change
made to the development metadata database is not propagated to the production
environment.

The development, staging, and production databases can exist in the same SQL
Server. If you change the name of the metadata database, you must specify the
name of the metadata database when you log on to the Conductor application or
when you change the metadata database.

### Connecting to a Local Metadata Database

As described in the *Dexterra Server Configuration Guide*, the default
installation of the Motorola Application Server assumes that the metadata
database is local, and resides in a SQL Server instance located on the same
server as the Motorola Application Server. This type of topology is shown in the
next graphic.

![Local Metadata Database - 2](media/65a97d491092ec4c9d9966280a1f0731.jpg)

#### Understanding Single-Server Installations

In testing environments, the metadata database is commonly located on the same
server as the Motorola Application Server. This simplifies the environment and
does not require an additional server. However, the drawback of locating the
metadata database on the same server as the Motorola Application Server is that
if the server (Server 1 as shown in [Connecting to a Local Metadata
Database](#connecting-to-a-local-metadata-database)) unexpectedly fails, the
Motorola Application Server and the metadata database become unavailable.

Using a distributed topology, as described in [Connecting to a Remote Metadata
Database](#connecting-to-a-remote-metadata-database), requires more
configurations but minimizes the risk of production down-time caused by hardware
failure.

#### Understanding Account Permissions for the Metadata Database

As described in the *Dexterra Server Installation Guide*, the local ASPNET
account is added as a user in SQL Server when you configure the metadata
database. This ASPNET account is the same account that runs the ASPNET process.

**Note:** Before you can log on to the Application Administrator tool, make sure
that the ASPNET account has db_datareader and db_datawriter access to the
metadata database. The ASPNET account needs to read the data to authenticate
users that log on to the Application Administrator tool. When changes are made
in the Application Administrator tool, this account must be able to write to the
database. The ASPNET account needs these permissions because by default, the
Application Administrator tool connects using Integrated Security.

##### Verify that the ASPNET account has sufficient permissions

1.  Start SQL Server Enterprise Manager from the Start menu.

2.  In the left pane, expand the node that corresponds to the instance of SQL
    Server that you want.

3.  Click the **Databases** node, and then the **MASMetadata** node.

4.  Under the MASMetadata node, click **Users**. The users associated with the
    database appear in the right panel.

5.  Right-click the ASPNET user, and click **Properties**. The **Database User
    Properties** dialog box appears.

![Adding New Motorola User to the SQL Server - 2](media/ddd36b248410dcdde5746bb8fb825cab.jpg)

1.  Select the following roles if they are not already selected.

-   Public

-   db_datareader

-   db_datawriter

1.  Click the **OK** button to save the changes.

### Verifying the Motorola Application Server Connectivity with the Metadata Database

The Motorola Application Server may connect to the metadata database using a
different account. The connection string is stored in the web.config file and
may be found in the physical directory of the Motorola Application Server. In a
default installation of the Motorola Application Server, the file is located in
the
[C:\\Inetpub\\wwwroot\\DexterraServer](file:///D:\Inetpub\wwwroot\%20MotorolaApplicationServer)
folder.

If the connection string is using Integrated Security, the ASPNET user is
employed and needs to be configured as described in [Verifying that the ASPNET
account has sufficient
permissions](#verify-that-the-aspnet-account-has-sufficient-permissions). If the
connection string is using a specific user to connect, then it is required that
the user should have the appropriate Read and Write permissions.

##### To assign Read and Write permissions

1.  Open SQL Server Enterprise Manager and expand **MASMetadata** from the
    **Databases** node.

2.  Under MASMetadata, click **Users**. The users associated with the database
    appear in the right panel.

3.  Right-click the user specified in the web.config file connection string, and
    select **Properties**. The **Database User Properties** dialog box appears.

4.  Select the following roles if they are not already selected:

-   Public

-   db_datareader

-   db_datawriter

1.  Click the **OK** button to save the changes.

#### Logging on to a Local Metadata Database

When you install the Motorola Application Server and log on to the Application
Administrator tool for the first time, the Application Server is configured to
use a local instance of the metadata database.

##### To log on to a local metadata database

1.  As defined in [Understanding Account Permissions for the Metadata Database,
    verify that the account permissions are correctly
    set.](#understanding-account-permissions-for-the-metadata-database)

2.  On your Web browser, navigate to
    <http://localhost/DexterraConductor/Login.aspx>.The **Application
    Administrator tool** login page appears.

>   Here, **localhost** is the name of the server hosting the Motorola
>   Application Server.

![App_Admin_Login_Page](media/05551a474b5697534aa2540eaa0506bc.jpg)

1.  In the **Username** box, enter the administrator username for the Motorola
    Application Server. Until changed, the default administrator username is
    **admin**. For more information, see [Changing the Default Administrator
    Account
    Credentials.](#changing-the-default-administrator-account-credentials)

2.  In the **Password** box, enter the administrator password. Until changed,
    the default administrator password is **password123**. For more information,
    see [Changing the Default Administrator Account
    Credentials](#changing-the-default-administrator-account-credentials).

#### Changing the Database Server

To change the database server that the Motorola Application Server and
Application Administrator tool access, you need to change the connection
information in the following places: the registry (for the Application
Administrator tool) and in the web.config file (for the Motorola Application
Server).

##### To change the database server

1.  On the Motorola Application Server computer, click the **Start** menu, and
    select **Run**. The **Run** dialog box appears.

2.  Enter **regedit** in the open box to start the Registry Editor.

3.  In the Registry Editor, navigate to the
    HKEY_LOCAL_MACHINE\\SOFTWARE\\Dexterra\\Studio key.

4.  Right-click **MetaDBConnectionString** and then click **Modify**.

5.  Change Data Source from **localhost** to the name of the database server you
    wish to use. For example if your remote server is called ProductionServer,
    change Data Source=localhost;Initial Catalog=MASMetadata;Integrated
    Security=SSPI **to** Data Source=ProductionServer;Initial
    Catalog=MASMetadata;Integrated Security=SSPI

6.  Using windows explorer, navigate to the physical web site directory for the
    Motorola Application Server. By default, this is
    C:\\Inetpub\\wwwroot\\DexterraServer.

7.  Open the web.config file for editing using a text editor, such as Notepad.

8.  An XML node called \<app settings\> is located at the bottom of the file.

9.  Change the **Data Source=localhost** to point to the server name. For
    example, if the remote server is called *ProductionSever*, then use **Data
    Source=ProductionServer** as the connection string.

10. Save the changes.

11. After making these changes, it is necessary to restart IIS. For this, click
    the **Start** button, and click **Run.** The Run dialog box appears.

12. Enter **cmd**, and click the **OK** button.

13. At the command prompt, type **IISRESET**, and press the **Enter** key to
    stop and restart IIS.

### Connecting to a Remote Metadata Database 

By default, the Motorola Application Server is configured to connect to the
metadata database on a local server, such as localhost. However, you can access
another database that is not on the same server as the Motorola Application
Server by changing the configuration information.

![Remote Metadata Database - 2](media/005123ab6d93d5087b877e9d083c4403.jpg)

#### Understanding Distributed Topologies

In a distributed topology, the metadata database is located on a server other
than the server hosting the Motorola Application Server. Distributed topologies
provide more failover points than single-box installations and are typically
used in production or staging environments.

Consider the scenario. If Server 1 in a remote metadata database unexpectedly
fails, it only affects the single instance of the Motorola Application Server
running on Server 1 and not the metadata database installed on Server 2.
Therefore, another instance of the Motorola Application Server could be used to
access and update the metadata database on Server 2, similar to the environment
depicted in high-availability topology. A distributed topology ensures that the
failure of a single server or a single piece of hardware does not affect your
entire environment.

#### Configuring a Remote Metadata Database

When configuring an environment to include a remote metadata database, you must
create a domain user account, which is then assigned permissions across all
resources. These resources include .NET resources, Motorola Application Server
resources, IIS resources, and SQL Server resources, and all servers.

#### Creating and Configuring the Domain Account

When creating and configuring a domain account, you first create a domain
account that will be used throughout the remaining procedures in this section.
For example: MYDOMAIN\\ASPUSER. Domain accounts are created on the Windows
server designated as the domain controller. Note that this server is not
depicted in Remote Metadata Database. You may need to contact your network
administrator to create the account.

For more information about creating a domain user account, see your Microsoft
2000 Server documentation. This user account is used to run the Motorola
Application Server. It will have permissions to the .NET resources and will be
assigned permission to the metadata database. This user account will also be
granted access to the Motorola Application Server application files.

**Note:** In the next procedure, it is assumed that Server 1 is the server
hosting Motorola Application Server and the IIS server. Server 2 is the server
hosting SQL Server and the metadata database. These reflect the topology in the
Remote Metadata database.

##### To create and configure the domain account

1.  On Server 1 (the server hosting the Motorola Application Server), click the
    **Start** button, and click **Control Panel**.

2.  Double-click **Administrative Tools**, and then double-click **Computer
    Management**.

3.  In the left panel, expand the **Local Users and Groups** folder.

4.  Click the **Groups** folder.

5.  In the **Look In** list, select the domain (for example, acme.com).

6.  Select **ASPNET** (ASPNET\@*mydomain*.com).

7.  Click the **Add** button.

8.  Click the **OK** button.

9.  In the Administrative properties window, notice acme\\ASPNET.

10. Click the **OK** button.

11. In the right panel, double-click **Log On As A Batch Job**. The **Local
    Security Policy Settings** dialog box opens.

12. Click the **Add** button.

13. In the Look In list, select **mydomain.com**.

14. Select the domain user account you created in step 1, and then click the
    **OK** button. In the Local Security Policy Setting window, notice that the
    Local Policy Setting and Effective Policy Setting columns are checked for
    *MYDOMAIN*\\ASPNET.

15. Click the **OK** button.

#### Assigning .NET Permissions to the Domain Account

The domain account user must be granted access to the .NET resources on Server
1. The domain account is MyDomain\\ASPUser for example.

##### To assign .NET permissions to the domain account

1.  On Server 1 (the server hosting the Motorola Application Server), start
    Windows Explorer.

2.  Assign the specified privileges to the domain account.

3.  Add the Domain User to the SQL Server Database Users. The domain account
    must also be granted access to the metadata database.

##### To add the domain user to the SQL Server database users

1.  On Server 2 (the server that holds the Metadata database), start SQL Server
    Enterprise Manager.

2.  In the left pane, expand the node that corresponds to the instance of SQL
    Server that you want.

3.  Click the **Databases** node and then the **MASMetadata** node.

4.  Right-click **Users,** and click **New Database User**. The Database User
    Properties - New User dialog box appears.

![Adding New Motorola User to the SQL Server - 2](media/0a4212fe52399f3bba6b13f4d0625c71.jpg)

1.  In the **Login name** box, select **\<new\>**. The SQL Server Login
    Properties dialog box appears.

![Adding New Motorola User to the SQL Server - 2](media/5985c8468a7d9c42fea9391ca5e13f0e.jpg)

1.  Next to the **Name** box, click the browse button. The SQL Server Login
    Properties dialog box appears.

2.  In the **List Names From** list, select the domain name to which the domain
    account belongs.

3.  Select the domain account, click **Add**, and click the **OK** button. You
    are returned to the SQL Server Login Properties - New Login dialog box.

4.  From the **Database** list in the Defaults section, select the name of the
    metadata database, such as **MASMetadata**, and click the **OK** button.

5.  In the Database User Properties dialog box, select the **public**,
    **db_datareader**, and **db_datawriter** options as shown in the following
    graphic.

![Adding New Motorola User to the SQL Server - 2](media/ddd36b248410dcdde5746bb8fb825cab.jpg)

1.  Click the **OK** button and restart SQL Server.

#### Logging on to the Remote Metadata Database

Once the user permissions have been configured, the final step is to log on to
the Application Administrator tool using the remote metadata database as the
metadata repository.

##### To log on to a remote metadata database

1.  Navigate to the Application Administrator tool URL:
    <http://localhost/DexterraConductor/Login.aspx>, where *localhost* is the
    name of the server hosting the Motorola Application Server. The login page
    appears.

2.  In the **Username** box, enter the administrator user name for the Motorola
    Application Server.

3.  In the **Password** box, enter the administrator password.

#### Changing a Metadata Database 

Although you can specify which metadata database to use when you log on to the
Application Administrator tool, you can also specify a different metadata
database to use from within the Application Administrator tool.

The metadata database is specified on the Security Settings form of the
Application Administrator tool. By default, this page is the first page to open
when you log on to the Application Administrator tool. You can change the
metadata database specified on the Security Settings page at any time.

**Note:** The next procedure assumes you are already logged on to the
Application Administrator tool. If you are not already logged on, you do not
need to change the metadata database as described in this procedure. Instead,
log on to the appropriate metadata database as described in [Logging on to a
Local Metadata Database](#logging-on-to-a-local-metadata-database).

##### To change the metadata database

1.  From within the Application Administrator tool, click **Settings** under the
    **Security** group in the left panel.

2.  In the **Server Name** box, enter the name of the server hosting the
    metadata database. For example, to switch your current settings to use a
    database on the same server as the Motorola Application Server instance,
    enter **localhost**.

3.  In the **Database Name** box, enter the name of the metadata database
    located on the server you specified in the Server Name box. In most cases,
    the name of the database is **MASMetadata**. For more information, see
    [Identifying the Metadata Database Naming
    Conventions](#identifying-the-metadata-database-naming-conventions).

4.  Save your changes by clicking the save icon. The Application Administrator
    tool pages are updated to reflect the metadata database you just specified.

#### Changing the Database Server

If you changed the name of the database server to something other than localhost
in the previous procedure, you also need to manually change the database server
that the Motorola Application Server is accessing.

To change the database server that the Motorola Application Server and
Application Administrator tool accesses, you need to change the connection
information in two places: the registry (for Application Administrator tool) and
in the web.config (for the Motorola Application Server).

##### To change the database server

1.  On the Motorola Application Server machine, click the **Start** menu, select
    **Run**.

2.  Enter the path to the regedit program. For example, enter **regedit**.

3.  Navigate to HKEY_LOCAL_MACHINE\\SOFTWARE\\Dexterra.

4.  Highlight **MetaDBConnectionString** and then right-click and choose
    **Modify**.

5.  Change the data source from localhost to the name of the database server.
    For example, if your remote server is called ProductionServer, change
    DataSource=localhost;Initial Catalog=MASMetadata;Integrated Security=SSP to
    DataSource=ProductionServer;Initial Catalog=MASMetadata;Integrated
    Security=SSPI.

6.  Using windows explorer, navigate to the physical web site directory for the
    Motorola Application Server. By default, this is:
    C:\\Inetpub\\wwwroot\\DexterraServer.

7.  Open the Web.Config file for editing. (Notepad will work as an editor.)

8.  An XML node called \<app settings\> is at the bottom of the file. In that
    node, find the connection string.

9.  Change the “DataSource=localhost” to the server name. For example, if the
    remote server is called ProductionSever, DataSource=ProductionServer in the
    connection string.

10. Save the changes.

11. After making these changes it’s necessary to restart IIS. Click the
    **Start** button, and click **Run**. The Run dialog box appears.

12. Enter **cmd**, and click the **OK** button

13. At the command prompt, enter **IISRESET** and press the **Enter** key to
    stop and restart IIS.

### Securing the Metadata Database

By default, the metadata database is secured using integrated security.
Integrated security uses the credentials of the account that runs the .NET
process to access the metadata database.

**Note:** You cannot modify the type of authentication that is used to secure
the metadata database. You can, however, use a different user account to access
the metadata database, as described in [Changing the Account that Runs the .NET
Process](#changing-the-account-that-runs-the-.net-process).

#### Identifying the Existing Account Used to Run the .NET Process

The name of the account used to run the .NET process is defined in the
machine.config file of the .NET framework files. By default, this file is
located in the following location.

C:\\WINDOWS\\Microsoft.NET\\Framework\\v1.1.4322\\CONFIG, where
C:\\WINDOWS\\Microsoft.NET\\ is the installed location of the .NET framework.

Within the machine.config file, there is a processModel section, as shown below:

\<processModel

enable="true"

timeout="Infinite"

idleTimeout="Infinite"

shutdownTimeout="0:00:05"

requestLimit="Infinite"

requestQueueLimit="5000"

restartQueueLimit="10"

memoryLimit="60"

webGarden="false"

cpuMask="0xffffffff"

userName="machine"

password="AutoGenerate"

logLevel="Errors"

clientConnectedCheck="0:00:05"

comAuthenticationLevel="Connect"

comImpersonationLevel="Impersonate"

responseRestartDeadlockInterval="00:09:00"

responseDeadlockInterval="00:03:00"

maxWorkerThreads="25"

maxIoThreads="25"

/\>

If the UserName variable is defined as **machine**, then the .NET process is
using the local ASPNET account that was located on the Windows 2000 server. The
full name of this account is typically, **aspnet_wp account**. The username is
typically, ASPNET.

This account must be granted access to the metadata database in the SQL Server.
You must also assign this user the **db_datareader** and **db_datawriter**
roles.

![Adding New Motorola User to the SQL Server - 2](media/5b3f9d5b960ab70df28c29ea3b283e2a.jpg)

#### Changing the Account that Runs the .NET Process

If necessary, you can modify the account that runs the .NET process and accesses
the metadata database. Generally, you do not need to do this unless you are
accessing the metadata database remotely and therefore, need to use a domain
account to access the metadata database located on a remote server.

##### To change the account that runs the .NET process

1.  On the server running the .NET process, navigate to the following location:
    C:\\WINDOWS\\Microsoft.NET\\Framework\\v1.1.4322\\CONFIG

2.  Using a text editor, such as Notepad, open the machine.config file.

3.  Navigate to the processModel node.

4.  Change the default userName variable from *machine* to the name of the
    domain account.

5.  Change the password variable from *auto generate* to the password used by
    the domain account. For example:

\<processModel  
enable="true"  
timeout="Infinite"  
idleTimeout="Infinite"  
shutdownTimeout="0:00:05"  
requestLimit="Infinite"  
requestQueueLimit="5000"  
restartQueueLimit="10"  
memoryLimit="60"  
webGarden="false"  
cpuMask="0xffffffff"  
userName="MYDOMAIN\\ASPUSER"  
password="password"  
logLevel="Errors"  
clientConnectedCheck="0:00:05"  
comAuthenticationLevel="Connect"  
comImpersonationLevel="Impersonate"  
responseRestartDeadlockInterval="00:09:00"  
responseDeadlockInterval="00:03:00"  
maxWorkerThreads="25"  
maxIoThreads="25"  
/\>

1.  Save the machine.config file with your changes.

### Exporting and Importing Data

The Motorola Import/Export utility enables you to import and export Dexterra
metadata in a readable XML format to and from a Motorola Application Server.
This functionality gives you an easy way to add or change business objects,
properties, business constants, views, or data sources for use by a revised or
similar but new client application.

Use the Export functionality to save metadata to an XML file. Use any text
editing tool, such as Notepad, to make changes (if necessary). After this, use
the Import functionality to import the file back to the same or a different
Motorola Application Server.

#### Exporting Data

When you export Dexterra metadata, the Motorola Import/Export feature creates an
XML document containing the metadata in a logical and hierarchical format. The
XML created is easily read and easily edited using a text editor. The Export
feature allows you export these objects.

-   Applications

-   Business objects

-   Commands

-   Connections

-   Data Objects

-   Views

-   Properties

-   Business rules

-   Event generators

-   Resources

-   Business categories and constants

-   System settings

-   Users

-   Groups

##### To export data

1.  Start the Application Administrator tool.

2.  Under the Utilities category in the left pane, select **Export**.

3.  In the Objects to Export group box, select the types of objects you want to
    include in the XML file. You can select one or multiple objects.

**Note:** If you select Application, the dependencies of the application, such
as business objects, properties, views, and so forth are *not* automatically
exported. If you want to export an application’s dependencies, you must
explicitly select them by clicking the appropriate dependency boxes.

1.  In the Export To group box choose whether you want to export the metadata to
    a file or to a different data source. Do *one* of the following:

-   To export to a file, enter the path and name of the XML file you want to
    create in the **File Name Including Path** box.

-   To export to a different data source, in the Server box, enter the name of
    the server on which the data source resides and then enter a valid username
    and password for that server.

1.  Click the **Export** icon.

**Note:** If duplicate objects are found during the Export, a warning message is
displayed. You can choose to continue or cancel. If you choose to continue, log
data is generated that lists all duplicate objects, their object types, and
their names under the logging category **Import/Export**. For more information
on setting the logging options, see [Configure the Logging Levels, History, and
Metrics
Collection](#configuring-the-logging-levels-history-and-metrics-collection).

#### Importing Data

After using the Export feature to create an XML file (containing all or select
pieces of your application’s metadata), you can import that XML file to the same
or a different Motorola Application Server.

##### To import data

1.  Start the Application Administrator tool.

2.  Under the Utilities category in the left pane, select **Import**.

3.  Do one of the following:

-   Type the path and name of the metadata XML file you want to import in the
    Import From box.

-   Click the **Browse** button to access the standard Windows Choose File
    window and navigate to the metadata XML file you want to import.

1.  Click the **Import** icon.

**Note:** If duplicate objects are found during the Import, a warning message is
displayed and you can choose to continue or cancel. If you choose to continue,
log data is generated that lists all duplicate objects, and their object types,
and names under the logging category **Import/Export**. For information about
setting logging options, see [Configure Logging Levels and Enable History and
Metrics
Collection](#configuring-the-logging-levels-history-and-metrics-collection).

#### Exporting Resources

If you select Resources, then your export file can get rather large since a copy
of all the resource files will be placed in the export file. By default, the
ASPNET process on the computer will have a size limit to the amount of data it
can handle in a single request. If the export file is larger than that, you
encounter an error message when importing. Typically the default maximum size is
set to 4096K (4M).

##### To configure the machine.config file to allow exporting of resources

1.  Open the machine.config file. In a default .NET Framework installation it is
    found at: C:\\WINDOWS\\Microsoft.NET\\Framework\\v1.1.4322\\CONFIG.

2.  Search for the node that begins with \<http runtime… There is a data element
    in this node called MaxRequestLength.

3.  Change that value from 4096 to a value big enough to allow resources to be
    exported.

4.  Once you are done with your import, it is probably best to reset this
    setting to its original value.

|                         | [./media/image2.jpeg](./media/image2.jpeg) |
|                         |                                            |
| Security Implementation |                                            |
|-------------------------|--------------------------------------------|


~   H2 logo

The Motorola Application Server provides security on several different levels
throughout the platform. The points at which authentication and security can be
implemented are shown in the following graphic and are described below.

![Security](media/da58801eb204ba4ededecf6d7e571f54.jpg)

The Motorola Application Server provides security for the following tasks.

-   **User Access to Application Data:** Users accessing data on mobile devices
    can be authenticated using IIS security or SOAP Authentication. SOAP
    authentication includes LDAP, Active Directory, and the Login Method. Users
    can also be disabled, which prohibits the user from accessing any data on
    their mobile device. For information about implementing security at this
    level, see [Securing User Access to
    Applications](#securing-user-access-to-applications).

-   **Access to Metadata Information:** The metadata database that stores
    business policy information is secured using SQL Server authentication. The
    Motorola Application Server uses services provided by .NET, and the user
    account that runs the .NET services is submitted to SQL Server for
    authentication when a connection to the MASMetadata database is attempted.
    The .NET account that runs the .NET services must be granted permissions to
    the MASMetadata database. For information about connecting to local and
    remote MASMetadata databases and configuring the permissions to the
    database, see [Securing the Metadata
    Database](#securing-user-access-to-applications).

-   **Access to Application Data Source**s**:** When the Motorola Application
    Server retrieves data, updates data, or accesses data to display in the
    Application Administrator tool, it must provide the appropriate credentials
    to the back end database. By default, the back end database is located on
    SQL Server. However, you can secure the back end application database using
    a variety of authentication methods, including IIS, database authentication,
    or no authentication at all.

### Securing User Access to Applications

When you request information from a mobile device, you are first authenticated
before you can retrieve or upload data. The type of authentication that can be
used to secure user access to an application includes the following:

-   IIS authentication

-   SOAP Authentication (LDAP, Active Directory, or the Login Method)

The type of authentication that is used is identified on the Server tab of the
Motorola Settings tool on the mobile device. However, the configuration of the
authentication is completed using the Application Administrator tool. The
Motorola Settings tool is shown in the next graphic.

![SOAP_Authentication](media/b54f07399e83c5b27987a34747d7454e.jpg)

#### Understanding the User Authentication Workflow

The Motorola Application Server authenticates the user each time a user makes a
request to upload or download data. The process of authenticating a user
includes several different tasks, which is shown in the following graphic and
described next.

![User Authentication Workflow - 2](media/2fc2e567676d156cd726c4fa0191099e.jpg)

1.  A user makes a request to retrieve the latest data.

2.  The Motorola Smart Client tool passes the user’s request and credentials
    over HTTP or HTTPS. The request can be sent over wireless protocols such as
    GSM/GPRS. Transmitting data over secure socket layers (SSL) provides
    additional security, although it may impact how quickly data is uploaded and
    downloaded.

3.  The Motorola Application Server receives the request and uses the .NET user
    account credentials to connect to the metadata database.

4.  The Motorola Application Server reads the business policies in the metadata
    database to determine where applications are located and what type of
    authentication is required for the applications.

5.  The Motorola Application Server does the following:

-   The server checks if the user has been authenticated by IIS, and if so,
    allows the request if the account is not disabled. If the account is
    disabled, the request is rejected.

-   If IIS authentication is not used, the server checks if SOAP header
    authentication is required. If neither IIS nor SOAP authentication is
    required, the request is allowed. This is because no authentication is
    required.

-   If SOAP header authentication is required, the server checks to see if the
    Login Method is enabled. If so, the server allows the request.

-   If the Login Method is not enabled, the server checks for a key in the SOAP
    header or a SoapAuthenticationHeader. If a key or SoapAuthenticationHeader
    is not found, the request is rejected.

-   If a key or SoapAuthenticationHeader is found, the server checks for Active
    Directory authentication requirements.

-   If Active Directory authentication is required, the server checks the user’s
    credentials and authenticates or rejects the request.

-   If Active Directory is not required, the server checks for LDAP
    authentication requirements.

-   If LDAP Authentication is required, the server checks the user’s credentials
    and authenticates or rejects the request.

1.  Once the user request is authenticated, the Motorola Application Server
    executes the necessary queries to retrieve the data requested by the user.
    The data is filtered based on business policies defined in the metadata
    database.

2.  The Motorola Application Server returns the data to the Motorola Smart
    Client, which then displays the information in the Dexterra mobile
    application.

### Configuring IIS User Authentication

IIS authentication enables the Motorola Application Server to authenticate the
user using Windows NT credentials. When integrated security is used, the user
who requests data via the mobile client application must have a valid domain
user account or an account with the local machine hosting the Motorola
Application Server. For example, if the Motorola Settings tool was configured
with the user name as **msmith**, then the server hosting the Motorola
Application Server must have a local account for *msmith*.

#### Understanding the Data Source Authentication Methods Compatible with IIS User Authentication

IIS user authentication requires that the IIS virtual directories used by the
Motorola Application Server are secured using basic authentication and
integrated security. Therefore, if you choose to use IIS user authentication,
you must secure the data source using integrated security.

#### Configuring IIS Authentication

When configuring integrated security, the procedures discussed in the following
topic must be completed.

#### Configuring IIS Directory Security

When integrated authentication is configured, you must use basic authentication
and integrated authentication on the Motorola Application Server virtual IIS
directories.

##### To configure IIS directory security

1.  From the **Start** menu, point to **Settings** and then click **Control
    Panel**.

2.  In **Control Panel**, double-click **Administrative Tools,** and then
    double-click **Internet Information Services**.  
    The Internet Services Manager console opens.

3.  Expand the server, Web Sites, and Default Web Site node.

4.  Right-click the DexterraConductor directory and select **Properties**.

5.  In the properties dialog box, click the **Directory Security** tab and in
    the **Anonymous Access and Authentication Control** check box, click
    **Edit**. The Authentication Methods dialog box appears.

![New Configuring IIS Directory Security - 3](media/98da8f01a6152c5a123c53a3f058bb90.jpg)

1.  In the **Authenticated Access** group box, select only the following check
    boxes.

-   **Basic Authentication**

-   **Integrated Windows Authentication**

    **Note:** Do *not* select Anonymous authentication.

1.  Click the **OK** button to save the settings.

2.  Click the **OK** button again to close the Properties dialog box.

3.  Repeat this procedure for the DexterraServer directory.

4.  Restart IIS (IIS Admin and World Wide Web Publishing) using the Services
    console. Access the Services console from the **Control Panel** by
    double-clicking **Administrative Tools**.

5.  Continue configuration as described in the next section, [Configuring
    Security Settings in the Application Administrator
    tool](#configuring-security-settings-in-the-application-administrator-tool-tool).

#### Configuring Security Settings in the Application Administrator tool tool

When using IIS authentication, you cannot configure the Motorola Application
Server to use LDAP or Active Directory authentication. Verify that these
settings have been set.

##### To verify security settings

1.  Start the Application Administrator tool.

2.  Under the **Security** category, select **Settings**.

3.  Verify the following:

-   **Database group box:** Do not modify this data, which reflects information
    that you entered when you configured the metadata database. For more
    information, see [Configuring the Metadata Database](#metadata-database).

-   **Motorola Application Server:** Do not modify this data. You entered the
    server name when configuring the metadata database, as described in
    [Implementing Security](#_Implementing_Security).

-   **Active Directory:** Do not enter information.

-   **LDAP:** Do not enter information.

-   **Authentication Method:** Leave SOAP Header Authentication unchecked.

-   **Authorization:** Leave Web Method Authorization unchecked.

1.  Click the **Save** icon.

2.  Create a Local User Account as described in the following.

#### Creating a Local User Account

If the DexterraConductor and DexterraServer virtual directories are secured
using Basic Authentication and Integrated Windows Authentication, as described
in the previous sections, then you must create a local user account on the
server that corresponds to each mobile client application user.

For example, if your application database has 50 users, including a user named
MSmith. Action items are assigned to those users. To log on to the application
as MSmith and see your data on the client device, you must create a local user
account on the DexterraServer for MSmith. The credentials must match those
defined in the application database. Now when you use MSmith as the device user,
the name is authenticated by IIS, and your application can use that same user
data to gather the correct action items for that user.

##### To create a local user account 

1.  From the **Start** menu, point to **Settings** and then click **Control
    Panel**.

2.  On the Control Panel, double-click **Administrative Tools.**

3.  In the Administrative Tools window, double-click Computer Management.

4.  In the **Computer Management** widow, expand Local Users and Groups.

5.  Right-click the **Users** node and select **New User**.

6.  Right-click the right panel window and select **New User**.

7.  In the **New User dialog** box, do the following:

-   In the **User name** box, enter a user name. For example, MSmith.

-   In the **Password** box, enter a password.

-   In the **Confirm Password** box, re-enter the password.

-   Make sure the **User must change password at next logon** box in cleared.

-   Select **User cannot change password** and **Password never expires**.

-   Click **Create**.

1.  Close all windows.

2.  Configure the SQL Authentication.

#### Configuring the Motorola Settings tool for IIS Authentication

Once the Motorola Application Server is configured for integrated security, you
must configure the Motorola Settings tool on Pocket PC also. The security
information is configured on the Server tab of the Motorola Settings tool.

##### To configure the Motorola Settings tool for IIS Authentication

1.  From the **Start** menu, point to **Programs**, and then click **Motorola
    Settings**.

2.  Click the **Server** tab.

3.  In the Web Services URL box, enter the hostname or IP address of the
    appropriate Motorola Application Server.

4.  Do one of the following:

-   For Authentication and Security, select **IIS Authentication.**

-   If the IIS Server hosting the Motorola Application Server has been
    configured for SSL, select **Secured Sockets Layer**. SSL provides increased
    security, although downloading and uploading data may take longer.

1.  Click **Apply** to save your settings. IIS authentication is now configured.
    When you specify an NT user on the **Config** tab of the Motorola Settings
    tool, and if the user requests data or uploads data, the Motorola
    Application Server authenticates the user who is employing IIS
    authentication.

#### Configuring SOAP/Active Directory Authentication

Configuring Active Directory authentication enables the Motorola Application
Server to authenticate users against a domain controller. When working with
Active Directory, the .NET process (aspnet_wp.exe) must run as a domain user.
Therefore, the machine.config file of the .NET framework must be modified to use
a domain account username and password, as described in this section.

**Important:** To secure the credentials passed in SOAP headers, enable SSL on
the IIS server hosting the Motorola Application Server and enable SSL on the
Motorola Settings tool on the mobile client devices.

The mobile client application user who has been authenticated against the domain
controller must also be defined in the dex_entity table of the Field Force
Automation data source. The credentials must be identical in the dex_entity
table, however, you do not need to provide the domain name. For example, if the
user name of the domain is **JSmith** and the password is **mypassword**, then
you must add a user with these credentials to the dex_entity table.

##### To configure Active Directory 

1.  Run the .NET Process as a Domain User.

2.  Enable SOAP Authentication.

3.  Configure the Application Administrator tool for Active Directory
    Authentication.

4.  Configure the Motorola Settings tool for SOAP Authentication.

5.  Add users to the Field Force Automation database and associate the users
    with tasks.

6.  Optionally, import users or users and groups, as described in [Understanding
    Import of Users and Groups](#importing-users-and-groups).

#### Running the .NET Process as a Domain User

The user account that runs the .NET process is identified in the machine.config
file, as described in [Identifying the Existing Account Used to Run the .NET
Process.](#identifying-the-existing-account-used-to-run-the-.net-process)

##### To run the .NET process as a domain user

1.  Open the machine.config file using a text editor. For more information on
    locating the machine.config and its contents, see [Identifying the Existing
    Account Used to Run the .NET
    Process.](#identifying-the-existing-account-used-to-run-the-.net-process)

2.  In the processModel node, locate userName="machine" and change it to
    userName="MYDOMAIN\\USER" where MYDOMAIN is the name of your domain and USER
    is the username.

3.  In the processModel node, locate password="AutoGenerate" and change it to
    password="password". Where password is the password assigned to the domain
    account.

4.  Save the changes, and close the machine.config file.

#### Configuring the Application Administrator tool for Active Directory Authentication

By configuring the Active Directory, you provide Motorola Application Server
with the information it needs to connect to the Active Directory and thereby
authenticate users.

##### To configure the Application Administrator tool for Active Directory

1.  Start the Application Administrator tool.

2.  Under the Security category in the left pane, select **Settings**. The
    Security Settings page appears. The Active Directory group box is shown in
    the following graphic.

![16_ActiveDirectory](media/e38b08e00934c42f99347fc1e5862990.jpg)

1.  Complete the following:

-   In the **Server** box, enter the name of the domain controller server.

-   Click the **Save** icon. The User Filter and Group Filter boxes are
    populated with default filters.

-   (optional) In the **User Filter** box, modify the filter used to specify
    which objectclass users are derived from. The value specified in this box is
    used when importing users and groups. It is not used for authentication
    purposes.

-   (optional) In the **Group Filter** box, modify the filter used to specify
    which objectclass groups are derived from. The value specified in this box
    is used when importing users and groups. It is not used for authentication
    purposes.

1.  Click the **Save** icon.

2.  Clear the cache as described in [Clearing the Cache](#clearing-the-cache).

3.  Add users from the Active Directory to the Field Force Automation database.

4.  In the **DB Login** box, enter the username of the SQL Server account that
    has been granted access to this data source.

5.  In the **DB Password** box, enter the password for the account.

6.  In the **Confirm Password** box, re-enter the password for the account.

### Configuring SOAP/LDAP User Authentication

Authenticating users employing LDAP authentication requires the use of basic
SOAP authentication. Basic SOAP authentication sends a SOAP header containing
the user’s credentials with each request for a Web method (this is a request to
upload or download data).

**Important:** To secure the credentials passed in the SOAP headers, enable SSL
on the IIS server that is hosting the Motorola Application Server. Also enable
SSL in the Motorola Settings tool on the mobile client devices.

#### Configuring LDAP User Authentication

Implementing LDAP user authentication includes the following steps:

1.  Configure Anonymous Access on the IIS Server.

2.  Configure the Application Administrator tool for LDAP Authentication.

3.  Enable SOAP Authentication.

4.  Configure the Motorola Settings tool as needed.

#### Configuring Anonymous Access on the IIS Server

When SOAP authentication is configured, you must use anonymous authentication
and disable Basic and Integrated Windows authentication. Anonymous
authentication must be configured for both the DexterraConductor IIS virtual
directory and the DexterraApplicationServer virtual directory.

##### To configure IIS directory security

1.  From the **Start** menu, point to **Settings** and then double double-click
    **Control Panel**.

2.  In the Control Panel, select **Administrative Tools**, and then **Internet
    Information Services**. The Internet Information Services console opens.

3.  Expand the Web Sites node and navigate to the DexterraConductor virtual
    directory.

4.  Right-click the DexterraConductor node and select **Properties**.

5.  In the properties dialog box, click the **Directory Security** tab.

6.  In the **Anonymous Access and Authentication** group box, click **Edit**.

7.  In the **Authenticated Access** group box, select **Anonymous access** and
    clear the **Basic Authentication** and **Integrated Windows Authentication**
    boxes.

![Configuring IIS Directory Security - 2](media/5cfe5e4ad43e438f062d733e3725ed88.jpg)

1.  Click the **OK** button. You are returned to the Properties dialog box.

2.  Click the **OK** button.

3.  Repeat this procedure for the DexterraServer virtual directory.

4.  Restart IIS (IIS Admin and World Wide Web Publishing) using the Services
    console. (Access the Services console from the **Administrative Tools** on
    the **Control Panel**.)

5.  Do one of the following:

-   Configure the Application Administrator tool for LDAP Authentication.

-   Configure the Application Administrator tool for Active Directory
    Authentication.

#### Configuring the Application Administrator tool for LDAP Authentication

LDAP authentication is configured on the Security Settings page of the
Application Administrator tool.

##### To configure the Application Administrator tool for LDAP Authentication

1.  Start the Application Administrator tool, if it is not already started.

2.  Under the Security category in the left pane, select **Settings**. The
    Security Settings page appears.

3.  Enter the following details.

-   **Server:** Enter the name of the server hosting the LDAP directory server.
    Optionally, append the port number (636 for SSL or 389 for non-SSL). For
    example, myserver:636. If you do not specify a port number, port 389 is used
    by default.

-   **Root node:** Enter the node of the location where Motorola Application
    Server will begin searching for users. For example,
    ou=People,dc=dexterra,dc=com.

-   **User Filter:** (optional) Enter a filter that identifies the objectclass
    from which users are derived. For example, (objectclass=inetorgperson).The
    value specified in this box is used when importing users and groups. It is
    not used for authentication purposes.

-   **Group Filter:** (optional) Enter a filter that identifies the objectclass
    from which groups are derived. For example,
    (objectclass=groupOfUniqueNames).The value specified in this box is used
    when importing users and groups. It is not used for authentication purposes.

-   **Member attribute:** (optional) enter a query using the name of an
    attribute found on a group object. You can authenticate and authorize users
    based on these attributes. For example, if your LDAP schema includes a group
    object that uses the attribute "businessCategory," then you could enter a
    member attribute of businessCategory=Technician to restrict access to data
    to only technicians.

1.  Click the **Save** icon.

2.  Clear the cache as described in [Clearing the Cache](#clearing-the-cache).

#### Enabling SOAP Authentication

Enabling SOAP header authentication allows the Motorola Application Server to
pass authentication credentials using SOAP headers. SOAP header authentication
is required when working with LDAP authentication, Active Directory
authentication, and Login Method authentication.

##### To enable SOAP header authentication

1.  Start the Application Administrator tool.

2.  Under the **Security category** in the left pane, select **Settings**. The
    Settings page appears.

3.  Select **Soap Header Authentication**.

4.  Click the **Save** icon.

5.  Configure the Motorola Settings tool for SOAP Authentication.

#### Configuring the Motorola Settings Tool for SOAP Authentication

When working with LDAP authentication, Active Directory authentication, or the
Login Method, you must enable SOAP authentication in the Motorola Settings tool.
Enabling SOAP authentication allows the Dexterra mobile client application to
send authentication information in SOAP headers.

##### To configure the Motorola Settings tool for SOAP authentication

1.  Start the Motorola Settings tool on the mobile device.

2.  Click the **Server** tab.

![abc copy](media/95ea4da1ed1161c6ad0d4d88f66ad266.jpg)

1.  Click the **SOAP Authentication** option.

2.  Optionally, if the IIS server hosting the Motorola Application Server is SSL
    enabled, select the **Secured Sockets Layer** check box.

3.  To accept the changes made, click the **Apply** button.

### Importing Users and Groups

Importing users and groups from an LDAP directory or Active Directory allows you
to configure the Application Administrator tool accounts for these users.
Importing users also provides you with the ability to enable and disable the
user accounts.

When you import a user or group, the user is added to the m_user table in the
MASMetadata database. Groups are added to the m_group table. When importing
users, the import process does not import passwords. Therefore, a user defined
in the m_user table is still authenticated against the LDAP directory or Active
Directory, where their credentials reside.

**Note:** If you import a user, you cannot change the user’s password using the
Application Administrator tool. The password is only defined in the LDAP
directory or Active Directory, and therefore, to change the password, you must
change it in LDAP or Active Directory.

##### To import users or users and groups

1.  Start the Application Administrator tool, if it is not already started.

2.  Under the Security category in the left pane, select **Settings**

3.  Do one of the following:

-   If you configured Active directory, then click the

    ![Icon_ActiveDirectory](media/2166bfebd54f1b79afb49009da92fcab.jpg)

    in the Active Directory group box to import only users or click

    ![Icon_ActiveDirectory](media/2166bfebd54f1b79afb49009da92fcab.jpg)

    to import users and groups.

-   If you configured LDAP, then click the

    ![Icon_ActiveDirectory](media/2166bfebd54f1b79afb49009da92fcab.jpg)

    in the LDAP group box to import only users or click

    ![Icon_ActiveDirectory](media/2166bfebd54f1b79afb49009da92fcab.jpg)

    to import users and groups.

1.  A confirmation message appears when the import process is complete.

**Note:** You must use a domain account in order to successfully import users
and groups. Make sure to update the machine.config file
(C:\\Windows\\Microsoft.NET\\Framework\\v1.1.4322\\CONFIG) in such a way that a
domain account is used when importing

#### Associating Imported Users with Administrator Permissions 

User accounts that have been imported from LDAP or Active Directory can be added
to a security group, which authorizes the user to access the Application
Administrator tool. However, a user must be added to a security group before the
user can log on to the Application Administrator tool; importing a user into the
m_user table does not automatically grant the user account the permissions to
log on to the Application Administrator tool. Depending on the security group to
which the user has been added, the user’s view of the Application Administrator
tool GUI varies. For more information about security groups and adding user
accounts to security groups, see [Working with Security
Groups](#working-with-security-groups).

#### Disabling Permissions for Imported Users

Any user that has been defined in the m_user table of the MASMetadata database
can be disabled. Therefore, importing users from LDAP or Active Directory into
the m_user table provides you with the ability to enable or disable these user
accounts. A disabled user is not authorized to access data on the Dexterra
mobile application, and when a disabled user attempts to access data, they are
alerted with a message.

**Note:** A status message appears notifying you if the account is active or
disabled, as shown in the following graphics.

![acc_still_active](media/684700bcfda8fa5d3257e35f50f4020e.jpg)

![acc_still_active copy](media/7d2d64c237d90088616d3a1aae93ccb4.jpg)

For more information about disabling user permissions, see [Disabling and
Enabling User Permissions](#disabling-and-enabling-user-permissions).

### Configuring the Login Method

The Login Method is an optional service that generates a unique session ticket
(GUID) for a user the first time they are authenticated by Active Directory or
an LDAP directory. When the user makes a subsequent request for a resource (such
as downloading or uploading data), the Login Method validates their session
ticket. Session tickets are passed in SOAP headers.

The Login Method provides a way to identify authenticated users without
requiring the Motorola Application Server to re-authenticate the user each time
the user makes a request. For example, if the Motorola Application Server
authenticates users against Active Directory, then the Motorola Application
Server only authenticates the user against the Active Directory the first time
the user makes a request. Once the user has the session ticket from the Login
Method, the Motorola Application Server does not need to connect to Active
Directory to re-authenticate the user.

Session tickets generated by the Login Method have a five-minute idle time out.
When the user makes the initial request, the session time out is set to five
minutes. As long as the user makes another request within the five-minute time
period, the session will be renewed for another five minutes. If the user does
not make another request within the five minutes, the session ticket expires.

If a user’s request contains an expired session ticket, then the user is
re-authenticated, and the Login Method sets a new session ticket.

##### To change the expiration duration of the login key in the m_setting table

1.  Using the Microsoft SQL Query Analyzer tool, use the Object Browser to drill
    to open the m_setting table.

2.  Change the LoginKeyExpiration value to change the session ticket idle time
    out.

##### To configure login method authentication

1.  Do one of the following:

-   Configure LDAP authentication, as described in [Configuring SOAP/LDAP User
    Authentication](#configuring-soapldap-user-authentication)

-   Configure Active Directory authentication, as described in [Configuring
    SOAP/Active Directory
    Authentication](#configuring-soapactive-directory-authentication).

1.  Configure the Motorola Settings tool to use Login Method.

#### Configuring the Motorola Settings Tool to use Login Method

The Login Method is specified on the Server tab of the Motorola Settings tool.

##### To configure the Motorola Settings tool to use Login Method

1. Start the Motorola Settings tool on the mobile device.

2. Click the **Server** tab to move it to the front.

The Server tab is shown in the following graphic.

![abc copy](media/95ea4da1ed1161c6ad0d4d88f66ad266.jpg)

1.  Select the **Use Login Method** box.

2.  Verify that **SOAP authentication** is selected. As stated above, the Login
    Method uses SOAP headers to store the session ticket. Therefore, SOAP
    authentication must be selected, and you can only use the Login Method with
    LDAP or Active Directory authentication.

3.  Click the **Apply** button to save the changes.

#### Understanding the Metric Collection for a Web Method

By default, the metrics for a Web method are collected. These are:

-   Time to download data from the back end system and put it into the DataSet

-   Time to read from the datastore in MASMetadata

-   Time to write to the datastore in MASMetadata

-   Time to compare two DataSets and build a third that contains the differences

-   Number of characters sent

-   Number of bytes received

-   Response time in milliseconds

##### To disable metric collection for a web method

1.  From the Web Methods page, click the Web method for which you want to
    collect metric data. The metrics available for collection are displayed in
    the Metrics tab.

2.  All metrics are collected by default. To disable collection of a particular
    metric, clear the **Enabled** check box for that metric.

### Clearing the Cache 

The Motorola Application Server caches some information that it uses in the
Application Administrator tool. When you make changes to the Security Settings
page, you must clear the cache after you save your changes.

There are two ways to clear the cache:

-   Using the Clear Cache option

-   Restarting the ASPNET process

##### To clear the cache using the Clear Cache button

After you save your changes on the Security Settings page, do one of the
following:

-   Click the **Clear Cache** option (under Utilities) in the left panel.

-   Press the **Alt + C** keys.

##### To clear the cache by restarting the ASPNET process 

1.  Start Windows Task Manager.

2.  Click the **Processes** tab to locate the aspnet process.

3.  Right-click the **aspnet_wp.exe** process and click **End Process Tree**.

4.  Close the Task Manager. The aspnet_wp.exe process restarts automatically.

| Users and Groups Configuration | [./media/image2.jpeg](./media/image2.jpeg) |
|--------------------------------|--------------------------------------------|


~   H2 logo

Users are created in the Application Administrator tool for certain reasons.
These are:

-   To associate the user with security groups, and allow the user to log on to
    the Application Administrator tool.

-   To associate the user with security groups, and allow or prohibit the user
    to call Web methods.

-   To provide you with the ability to enable or disable users.

When you create a user using the Application Administrator tool, the user is
added to the m_user table of the MASMetadata database. By default, when you
first configure the MASMetadata database, as described in the *Dexterra Server
Installation Guide*, one user is added to the m_user table, and this user is the
default Administration user (username is **admin** and password is
**password123**).

### Importing verses Creating Users

As described in [Importing Users and Groups](#importing-users-and-groups), users
can be imported into the m_user table from Active Directory or an LDAP
directory. When a user has been imported into the metadata database, only the
username is imported into the m_user table. The password is not imported into
the metadata database.

When you create a user in the Application Administrator tool, the user’s
password is included in the m_user table. This password can be changed using
Application Administrator tool.

### Creating Users

Users are created on the Users page of the Application Administrator tool.

##### To create users

1.  Start the Application Administrator tool, if it is not already started.

2.  Under the **Security** category, select **Users**. The Users page opens.

3.  If the User boxes are not blank, click

    ![Icon_3](media/aeb10cc5a85866d291f42d9e12ca10ed.jpg)

    to empty the values in the boxes.

4.  Complete the following boxes:

-   **User ID**: Enter an The user will log on to the Application Administrator
    tool using this ID.

-   **Password**: Enter the user’s password.

-   **Confirm Password**: re-enter the user’s password.

-   **First Name**: optionally, enter the user’s first name.

-   **Last Name**: optionally, enter the user’s last name.

-   **Display Name**: optionally, enter the user’s complete name.

-   **Email**: optionally, enter the user’s e-mail address.

-   **Telephone**: optionally, enter the user’s telephone number.

-   **Description**: optionally, enter a description of the user.

1.  Optionally, select the **Disabled** box to disable the user.  
    Once disabled, a user cannot log on to the Application Administrator tool or
    start the Dexterra mobile client application.

2.  Do one or more of the following:

-   Click the save icon to save the user to the m_user table in the MASMetadata
    database.

-   Click the save icon to save the user to the m_user table in the MASMetadata
    database and clear the boxed to enter another user account.

1.  If the user is an Administrator, be sure to add the user to the
    Administrator group as described in [Adding Users to
    Groups](#adding-users-to-groups).

Users will not be permitted to log on to the Application Administrator tool
unless they are part of the Administrator group.

#### Deleting Users

Deleting a user removes the user’s account from the m_user table. Once deleted,
the user cannot access the Application Administrator tool.

##### To delete users 

1.  Start the Application Administrator tool, if it is not already started.

2.  Under the **Security** category, select **Users**.

3.  Do one of the following:

-   Click **Delete** next to the user you want to remove.

-   Click the user name to display the user’s information and click the delete
    icon.

1.  At the confirmation prompt, click the **OK** button to delete the user.  
    The user’s record is removed from the m_user table in the MASMetadata
    database.

#### Changing User Passwords

You can only change the password of a user that was created using the
Application Administrator tool. You cannot change the password of a user that
was imported into the metadata database from Active Directory or an LDAP
directory.

##### To change a user’s password

1.  Start the Application Administrator tool, if it is not already started.

2.  Under the **Security** category, select **Users**.

3.  Click the name of the user whose password must be changed. The user’s
    information appears in the User box.

4.  Next to the **Password** box, click the **Change** button. The Change
    Password page opens.

5.  Do one of the following:

-   **Old Password**: enter the current password.

-   **New Password**: enter a new password. Passwords must be less than 25
    characters. Passwords can be blank.

-   **Confirm Password**: re-enter the new password.

1.  Click **Submit**.

### Disabling and Enabling User Permissions

Disabling an account prohibits the user from downloading data, uploading data,
launching the Dexterra mobile client application, and logging on to the
Application Administrator tool. Users that are defined in the m_user table of
the MASMetadata database can be disabled and enabled using the Application
Administrator tool. The status of a user can be verified using the Motorola
Settings tool.

#### Verifying User Status

The status of a user can be verified on the Config tab of the Motorola Settings
tool.

##### To verify the status of a user

1.  Start the Motorola Settings tool on the mobile client device.

2.  Click the **Config** tab.

3.  In the User Name box, enter the name of the user of interest.

4.  In the User Password box, enter the user password.

5.  Click the status button to check the status of the account.

**Note**: A status message appears notifying you that the account is active or
disabled. This is shown in the next graphic.

![acc_still_active](media/684700bcfda8fa5d3257e35f50f4020e.jpg)

![acc_still_active copy](media/7d2d64c237d90088616d3a1aae93ccb4.jpg)

##### To enable or disable user permissions

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Users**.

3.  Click the name of the user you wish to disable or enable.

4.  Do one of the following:

-   To disable the user, select the **Disable** check box.

-   To enable the user, deselect the **Disable** check box.

1.  Click the **Save** icon.

### Working with Security Groups

By default, there are three categories of security groups. These are:

-   Developer

-   Analyst

-   Admin

In addition to working with these three default security groups, you can create
your own custom groups as described in [To Create a Security
Group](#to-create-a-security-group). Each of these groups is associated with a
different set of administrative views. These groups dictate the administrative
options available to a user when they log on to the Application Administrator
tool. Administrative options appear on the left side of the Application
Administrator tool GUI as shown in the next graphic.

![02_SecurityGroupAdministrativePrivileges](media/3cc3187ebfce8bd2450cde782e54faaf.jpg)

#### Understanding the Administrator Security Group

When IIS authentication is used, the Motorola Application Server automatically
grants any user who is a member of the IIS Administrator account the same rights
as a user who is a member of the Administrator security group.

##### To create a security group

1.  Start the Application Administrator tool.

2.  Under the Security category, click **Groups**. The Groups page opens.

3.  In the Name box, enter the name of the new group.

4.  In the Description box, enter a narrative of the new group.

![create security grp](media/34a1593d421cfe4d7758afc31a257ebd.jpg)

1.  Click the **Save** icon to save the new group.

2.  Perform one or more of the following:

-   Define group permissions.

-   Add sub-groups.

-   Assign users to the group.

#### Assigning Permissions to a Security Group

Once a security group has been created, you must assign permissions to the
group. Anyone then assigned to the group will inherit the permissions assigned
to the group.

##### To assign permissions to a security group

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Groups**.

3.  On the Groups page, select the name of the group to which you want to add
    permissions.

![To assign permissions to a security group](media/ae20fe3b3e8a9bda0ae14691902a3234.jpg)

1.  At the bottom of the Groups page, click the **Permissions** tab.

2.  Click the **Add** box next to the appropriate permissions.

![assign permissions to a security group ](media/148c1bc2a7bd7966f54b69498a1eebcd.jpg)

1.  Click **Add** to add the permissions to the group definition.

#### Adding Sub-groups to a Group

Sub-groups inherit the permissions and Web methods from their parent group. For
example, if you select Administrator and add a sub-group called Analyst to this
group, then Analyst inherits all the permissions and Web methods assigned to the
Administrator.

Consider your security policies before adding sub-groups to a group. Do not add
a sub-group to a group if the sub-group should not have the same permissions as
the group.

##### To add a sub-group to a group

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Groups**.

3.  On the Groups page, select the name of the parent group to which you want to
    add permissions.

![To add a sub-group to a group](media/2fcfcd227b80e5dc22e6de917d9c1d5e.jpg)

1.  Click the **Sub-groups** tab.

2.  From the **Sub-groups** list menu, select the group to add to the current
    group.

3.  Click **Add**. The sub-group is added to the group.

#### Removing a Sub-Group from a Group

Once you have added a sub-group to a group, you can remove the sub-group from
the group at any time. Removing a sub-group from a group removes the sub-group’s
permissions and Web methods that it inherited from the group.

##### To remove a sub-group from a group

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Groups**.

3.  On the Groups page, select the name of the group from which you want to
    remove a sub-group. Information about the group displays in the page as
    shown in the following graphic.

![22_Groups](media/b41e8569ca8f5aeff042e21a9c8ab4f9.jpg)

1.  Click the **Sub-Groups** tab.

2.  Click **Remove** next to the sub-group you want to remove. The sub-group is
    removed from the group.

#### Adding Users to Groups

Users are added to a group to provide the user with the permissions and Web
methods assigned to the group.

##### To add users to a group

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Groups**.

3.  On the Groups page, select the name of the group to which you want to add
    users.

4.  Click the **Users** tab.

![22_Groups_UsersTab](media/5be6d99413d69d9667a1359f3fe7a8bc.jpg)

1.  From the **Users in Groups** list, select a user to add to the group.

2.  Click **Add**. The user is added to the group.

#### Removing Users from Groups

Users that have been added to a group can also be removed from the group.

##### To remove users from groups

1.  Start the Application Administrator tool.

2.  Under the **Security** category, click **Groups**.

3.  On the Groups page, select the name of the parent group from which you want
    to remove users.

![To remove users from groups](media/1a38ef36fb85fac3139e5970eb59c334.jpg)

1.  Click the **Users** tab.

2.  Next to the user you want to remove, click **Remove**. The user is removed
    from the group.

| Configure the Logging | [./media/image2.jpeg](./media/image2.jpeg) |
|-----------------------|--------------------------------------------|


~   H2 logo

The Motorola Application Server automatically collects log history. It can also
log Web service metric data if it is configured to do so. This allows you to
monitor the transactions that take place and to troubleshoot issues. You can log
any of the services that comprise the Motorola Application Server and log
metrics for the Web methods used by the Web services.

Logging information is stored in the m_log table of the MASMetadata database.
Metrics are stored in the m_metric table.

#### Configuring Client-Side Log Information

In addition to capturing server log information, client-side log information is
also captured saved to a file named log.txt. This file is located on the device
in the Dexterra folder. If users contact your Support personnel with issues,
instruct them to navigate to the log.txt file, and open it. This is the first
act of troubleshooting.

#### Configuring the Logging Levels, History, and Metrics Collection

The Log Settings page is used to specify that the Motorola Application Server
collect log history and Web method metric data.

##### To configure logging levels and enable history and metrics collection

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Settings**. The Log
    Settings page opens. The Log Levels group box is shown.

3.  For each category, select the level of message description to capture and
    display in the Logs screen. By default, the message description level for
    all Web services is set to "Error." Choose from:

-   **Error:** This logs only error messages.

-   **Important:** This logs only error and warning messages.

-   **Information:** This logs error, warning, and information messages.

-   **Verbose:** This logs error, warning, information, and verbose messages.

    **Note:** The level of logging may negatively impact server performance
    depending on the amount of logging that occurs. Log size is limited only by
    the amount of disk space where the MASMetaData database is located.

1.  Do one of the following:

-   To save the log file to the cache, make sure the **Caching** option is
    selected. Clear this option if you do not want to save the log file to the
    cache.

-   To enable the server to collect measurements (such as bytes received,
    characters sent, and response time) for all Web service Web methods, click
    the **Turn ON all Metrics** button.

>   **Note:** If you choose to use all Metrics, and subsequently turn off metric
>   collection for one or more Web methods, the **Turn On all Metrics** button
>   is toggled off automatically. Similarly, if you choose to turn off all
>   Metrics, and subsequently turn on metric collection for one or more Web
>   methods, the **Turn Off all Metrics** button is toggled off automatically.
>   In these instances, the Status message provides additional information.

-   To view the logs, see [Viewing Log Information](#_View_Log_Information).

### Understanding Conflict Notifications

A conflict can occur when two records with the same primary key both contain
different data. During synchronization, the Motorola Application Server compares
records received from the client against the MASMetadata database to synchronize
changes and detect conflicts. For example, at 10:30 AM Field Representative John
changes customer Acme Products Company’s phone number using his Pocket PC field
application. He then successfully synchronizes the change to the MASMetadata
database. At 10:45 AM, of that same morning Field Representative Sam (who has
not synchronized since 10:00 AM) also changes Acme’s phone number. When he
attempts to synchronize, the Motorola Application Server notes that his record
is old, compares his version to the newest version and can email a conflict
notification to interested parties.

Timestamp comparison is not the only option when it comes to detecting record
conflicts. The conflict detection method is determined on a per client table
object basis by your application developer or database administrator using the
Application Administrator tool. For information about configuring the conflict
detection method and the conflict resolution method, see the *Dexterra Server
Configuration Guide*.

The section, [Understanding Conflict
Resolution](#understanding-conflict-resolution), briefly describes the available
conflict resolution methods. If the application developer or database
administrator has selected Manual Resolution, the *first in* data prevails.
However, as an administrator, you are responsible for reviewing the conflicting
data and, if indicated, overriding the First In, First Out (FIFO) conflict
resolution. For instructions, see [Viewing and Resolving
Conflicts](#viewing-and-resolving-conflicts). The next section describes how to
specify recipients for a conflict notification email.

#### Configuring Conflict Notification for Senders and Recipients

The Log Settings page is used to specify the recipients of any conflict
notification emails that may need to be sent. A sample email conflict
notification is shown below.

##### To configure conflict notification for senders and recipients 

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Settings**. The Log
    Settings page opens. The Conflicts group box is shown.

3.  In Sender Email, enter the email address of the individual or group from
    whom the conflict notification will be sent.

4.  In Recipient Email, enter the names of all individuals who should be sent
    notification of record conflicts. Separate multiple email addresses with a
    semicolon (;).

5.  Check **Include User** to also send a record conflict notification to the
    user who introduced the conflict.

### Viewing Log Records

The Logs page displays information about all logs currently stored in the log
file. The logs can be sorted by log level, category, server name, thread ID,
timestamp, or the IP address. To maintain a more meaningful log, you can delete
any records containing a specific log level, category, server name, user name,
thread ID, or timestamp.

##### To view log information

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page
    opens. By default, log records are sorted by timestamp.

##### To sort the log 

**Note:** You can sort the log alphabetically (in descending or ascending
order). You can also sort by level, category, server, user, thread ID, or
timestamp. Click the appropriate column name and then click for a second time to
sort the column in the opposite order.

##### To limit records displayed in the log

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page
    opens.

3.  In the **Page Size** textbox, enter the number of log records that will be
    recorded to a page, for printing purposes. The minimum size is 100 and the
    maximum is 500.

4.  To show only those logs matching a specific level, category, server name,
    thread ID, or timestamp, specify the unique search criteria in the text box
    above the appropriate column heading. (The format must match the data
    format. For example, timestamp must use the format mm-dd hh:mm:ss where the
    time portion is in GMT format). In the case of level or category, select
    from the drop down. Click the **Find** icon.

5.  To redisplay all log records, set the level and category lists to the blank
    selection (at the top of the list selections) and clear the server, message,
    thread ID, and timestamp text boxes.

6.  Click the **Find** icon.

##### To export the log to a delimited .txt file

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page
    opens.

3.  (Optional) To show only those logs matching a specific level, category,
    server name, thread ID, or timestamp, specify the unique search criteria in
    the text box above the appropriate column heading. (The format must match
    the data format. For example, timestamp must use the format mm-dd hh:mm:ss
    where the time portion is in GMT format). In the case of level or category,
    select from the drop down. Click the **Find** icon.

4.  Click the Export icon.

5.  In the **Export Log by Search Criteria dialog** box, click the **OK**
    button.

6.  In the **File Download** dialog box, click **Save**.

7.  In the **Save** dialog box, navigate to the directory to which you want the
    log file downloaded, name the log file, and then click the **Save** button.

##### To permanently delete records from the log

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Logs**. The Logs page
    opens.

3.  To permanently delete log records matching a specific level, category,
    server name, thread ID, or timestamp, specify the unique delete criteria in
    the text box above the appropriate column heading. (The format must match
    the data format. For example, timestamp must use the format mm-dd hh:mm:ss
    where the time portion is in GMT format). In the case of level or category,
    select from the drop down.

4.  Click the **Delete** icon.

### Viewing Web Service Web Method Metrics

You can view data on the metrics collected by the logger for each Web method
used by each Web service. See the next section for help in deciphering this
data.

Metrics collected include the average, minimum, maximum, total, sample size, and
date and time last called for the following:

-   **Bytes Received** - For each "send" to the Web method, Bytes Received
    indicates the number, average, minimum, etc. of bytes received by the Web
    method.

-   **Characters Sent** - For each "send" to the Web method, Characters Sent
    indicates the number, average, minimum, etc. of bytes sent.

-   **Response Time (in milliseconds)** – This indicates the number, average,
    minimum, etc. time taken by the Motorola Application Server to process the
    request and send a response.

##### To view metric data for each method associated with a Web service

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Metrics**.

#### Interpreting the Web Service Web Method Metric Data

The Response Time metric indicates how long the Web method took to execute minus
the time spent transmitting data to the Web server and back from the Web server.
In general, for a dedicated server, acceptable response time should average 500
milliseconds.

**If response time is high**, then the execution of the Web method logic may be
the bottleneck. If there are no indications of network capacity problems, then
the problem may be inefficient code within the Web method or, more likely,
delays inherent in accessing external data sources. A common problem is SQL
queries that result in full-table scans. A Database Administrator can run a SQL
trace and determine the efficiency of the query being executed. It may be, for
example, that adding an index greatly reduces the response time. If at all
possible, it is best to separate the actions the Web method is performing, and
run them individually to judge the response time of each and determine the
bottleneck. However, this may not be possible without the source code.

**If response time is low**, and no other operations appear to be the
bottleneck, then the transmission of information back and forth over the network
may be the problem. It also may be helpful to check the size of the packets sent
to and received back from the Web server. If the packet sizes are large, it will
obviously take longer to transmit. Even if the packet sizes are small, you may
want to investigate network capacity. If the network is near its maximum
capacity, then the performance of all operations over the network is likely to
be impaired until capacity is added or utilization is reduced. In the specific
case of large packet sizes, it is possible that too much data is being sent or
retrieved (more likely retrieved). If the Web method is bringing back some sort
of result set, consider constraining the data further.

**If bytes received, characters sent, and response time are all high**, consider
researching server latency to determine whether server load is affecting
performance.

### Viewing History

The History page shows, for a particular user (client), calls to all or specific
user table objects, and the attributes, and attribute values associated with
that object. For each call, you can drill to view client and server
synchronization time data, revision information, and view the associated primary
key(s).

##### To view calls to user table objects

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **History**. The History
    page appears.

3.  In the **Select User** list, select a user.

4.  In the **Select View** list, select a client user table object, or select
    **All**.

5.  Click the **Find** icon. The History page redisplays with information about
    the requested client user table objects.  
    For each object, the tables display associated attributes, the date and time
    when those attributes were updated, and each attribute’s new value.

6.  To view additional details about a particular object call, click a timestamp
    hyperlink. The History Record page opens. The History Record page displays
    the following additional information about the selected object call:

-   **Client Time:** This displays the date and time the object was called from
    the client.

-   **Server Time:** This displays the date and time the object call reached the
    server.

-   **Revision:** This displays the number of times this object value has
    changed.

-   **Primary Key(s):** Lists the attribute(s) used as the object primary key.

### Understanding Conflict Resolution

Once the Motorola Application Server determines that an object value update
conflict has occurred, the conflict is resolved using one of three methods
selected for that object by the developer or database administrator. These
methods are:

-   **First Update Wins** (Preferred method)**:** In this scenario, the Server
    only accepts the first update to a record and rejects any update attempts
    made by an unsynchronized client. Unsynchronized client updates in which a
    conflict is detected by the database, will be dropped and the "first update"
    (server) version is returned to the client. This method ensures that an
    unsynchronized client cannot overwrite a valid, updated record.

-   **Last Update Wins:** In this scenario, the Motorola Application Server does
    not need to detect conflicts. It simply accepts the last version provided by
    any client, and overwrites any prior change that may have been made.

-   **Administrator (Manual) Resolution:** In this scenario, all object update
    conflicts are treated as errors. The designated parties are alerted via
    e-mail and the administrator determines, case by case, which update wins.

#### Viewing and Resolving Conflicts 

As an administrator, you can view a list of conflicts queued for manual
resolution. As new conflicts arise, you can also be sent an e-mail notification.
For details, see [Understanding Conflict
Notifications](#understanding-conflict-notifications).

##### To view conflict details and select the object value that prevail

1.  Start the Application Administrator tool.

2.  Under the Logging category in the left pane, select **Conflicts**. The
    Conflicts page opens.

3.  Click a **Resolve** link to display details about that conflict.

4.  Click the update in the Current column to highlight it and display
    additional information about the conflict. Click a *username* (*\#*) column
    to the right of the Current column to highlight it. Review the data in the
    columns to determine which update should prevail.

5.  To select the winning update, highlight that column and click the **Save**
    icon.

6.  Continue the steps above to resolve additional record conflicts.

#### Initializing Logging on the Client Application

With this release, there is a client logging feature that writes debug
information to a log file on the Pocket PC. For details about the code change
needed in your Pocket PC application to accommodate this functionality, see
[Defining Business Objects](#defining-business-objects).

|                                            | [./media/image2.jpeg](./media/image2.jpeg) |
|                                            |                                            |
|                                            |                                            |
| Appendix: Sample Server-Side Business Rule |                                            |
|--------------------------------------------|--------------------------------------------|


~   H2 logo

The following business rule monitors the contents of the a_messagequeue table
for null d_sent column values. In this example, a null value indicates that a
new table record has been added. For each new record row, a custom Web Service
Web method takes the s_from, s_to, s_subject, and s_body values, constructs an
e-mail message, and sends it to the s_to recipient.

'Imports Dexterra.Client

Imports Dexterra.Server

Imports Dexterra.Server.BusinessRule 'Required to create a business rule.

Imports Dexterra.Server.Common

Public Class SMSBusinessRule

Implements IBusinessRule 'Implementation of this interface is required.

Public Const SQL_CONN_STR = "Provider=SQLOLEDB;Data  
Source=localhost;Initial Catalog=FSASP1;Integrated  
Security=SSPI;"

Public Const SQL_GET_COUNT = "select count(k_messagequeue) from  
a_messagequeue where d_sent is null" 'a_messagequeue is a custom  
’table in which SQL code is stored; d_sent is a column in  
’that table. Because the information is static, it can be  
’stored as constants.

Public Const SQL_GET_ITEM = "select k_messagequeue,  
s_from=isnull(s_from, ''), s_to=isnull(s_to, ''),  
s_subject=isnull(s_subject, ''), s_body=isnull(s_body, '')  
from a_messagequeue where d_sent is null"

Public Const SQL_UPDATE_ITEM = "update a_messagequeue set  
d_sent = getdate(), d_messagequeue_update = getdate(),  
k_user_update = -2 where k_messagequeue = "

Public Const WSSMTP_IP = "localhost"

Public Const WSSMTP_FILE = "/WSSMTP/SendSmtp.asmx"

Public Function Evaluate() As Boolean Implements  
IBusinessRule.Evaluate 'Business rules must have Evaluate and  
’Execute methods.

Dim count As Int32

count = Common.OleDb.ExecuteScalar(SQL_CONN_STR,  
SQL_GET_COUNT)'ExecuteScalar is a  
’custom method that executes SQL code.

Return (count \> 0)

End Function

Public Sub Execute() Implements IBusinessRule.Execute

'Business rules must have Evaluate and Execute methods.

Dim k_messagequeue As String

Dim s_from As String

Dim s_to As String

Dim s_subject As String

Dim s_body As String

Dim s_update As String

Dim myURL As String

Dim mySMSFileName As String

Dim s_return As String

Dim mySMTP As localhost.SendSMTP 'SendSMTP is a custom Web service.

Dim i As Int32

Dim results As IList

Dim vals As System.Object()

Try

 MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,Common.Constants.BUS_RULE_LOG_CATEGORY,
"IN EXECUTE") ’WriteLine is a custom method that  
’writes messages to the Dexterra Application 'Server log.

mySMTP = New localhost.SendSMTP

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,Common.Constants.BUS_RULE_LOG_CATEGORY,
"Loading content")

myURL = MetaData.BusinessConstantCache.instance.Item("SMSServer","SMSIP") 'This
provides access to business constants ’on the Dexterra Server. (Business
constants are ’defined in the Dexterra Conductor.)

If (myURL.ToString() = "") Then

myURL = WSSMTP_IP

End If

mySMSFileName =
MetaData.BusinessConstantCache.instance.Item("SMSServer","SMSFile")

If (mySMSFileName.ToString() = "") Then

mySMSFileName = WSSMTP_FILE

End If

'build Full WebServicer URL/File

myURL = "http://" & myURL & WSSMTP_FILE

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,  
Common.Constants.BUS_RULE_LOG_CATEGORY, "execbusrule", "URL  
was " & mySMTP.Url.ToString)

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,  
Common.Constants.BUS_RULE_LOG_CATEGORY, "execbusrule", "URL  
is " & myURL.ToString)

results = OleDb.ExecuteReader(SQL_CONN_STR, SQL_GET_ITEM)

'ExecuteReader is a Dexterra custom method that executes SQL code.

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,  
Common.Constants.BUS_RULE_LOG_CATEGORY, "execbusrule",  
"found " & results.Count.ToString & " row")

For Each vals In results

'// initialize variables

k_messagequeue = ""

s_from = ""

s_to = ""

s_subject = ""

s_body = ""

s_update = ""

'load each string

k_messagequeue = CType(vals(0), String)

s_from = CType(vals(1), String)

s_subject = CType(vals(2), String)

s_to = CType(vals(2), String)

s_subject = CType(vals(3), String)

s_body = CType(vals(4), String)

' set the URL to the proper location that we set above

mySMTP.Url = myURL.ToString()

If k_messagequeue \<\> "" And s_from \<\> "" And s_to \<\> "" Then

'send it

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,  
Common.Constants.BUS_RULE_LOG_CATEGORY,  
"execbusrule", "about to send: " & s_from & " " & s_to  
& " " & s_subject & " " & s_body)

s_return = mySMTP.Send(s_to, s_from, s_subject, s_body)

'Send is a custom Web method.

If CBool(s_return.ToString) Then

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,Common.Constants.BUS_RULE_LOG_CATEGORY,
"execbusrule","about to update " & k_messagequeue)

s_update = SQL_UPDATE_ITEM & k_messagequeue

OleDb.ExecuteScalar(SQL_CONN_STR, s_update)

End If

End If

Next

Catch ex As Exception

MetaData.Logger.instance.WriteLine(TraceLevel.Verbose,Common.Constants.BUS_RULE_LOG_CATEGORY,
"execbusrule", "SMS Business Rule Exception " & ex.Message)

End Try

End Sub

End Class

<br>Index
---------

A

abbreviations, 3

accounts

Application Administrator tool, 7

acronyms, 3

active directory authentication

configuring

Application Administrator tool, 56

configuring Application Administrator tool, 56

adding

new business objects to your small factor application, 23

sub-groups to security group, 70

users to group, 72

adding a new business object to an application

How to, 23

adding domain user

SQL Server database users

How to, 41

adding sub-groups to a security group

How to, 70

adding users to groups

How to, 72

administrative tasks, 10

administrator credentials

changing, 9

Administrator security group, 69

agile controls

AgileTenKey, 13

AutoPersist property, 13

binding data, 13

Edit property, 13

AgileTenKey control, 13

analyzing

business categories and constants, 27

appendix

sample server side business, 80

architecture

Motorola Application Server, 6

assigning .Net permissions

How to, 41

assigning permissions

security groups, 69

assigning permissions to security groups

How to, 69

assigning read and write permissions

How to, 37

associating imported users and groups

administrative permissions, 61

audience, 2

authentication

data source, 52

authentication of users

workflow, 51

AutoPersist property

agile controls, 13

B

binding data, 13

business categories and constants

analyzing, 27

business object events

initiating, 31

business objects, 15

understanding, 15

business rule resource

creating, 23

business rules

creating, 25

defining, 25

invoking, 25

business rules and constants, 25

business rules in the Application Administrator tool

defining, 27

C

cache

clearing, 63

changing

account that runs.Visual Studio .Net account

How to, 47

account to run Visual Studio.Net process, 47

database server, 38, 45

default administrator credentials, 9

metadata database, 44

user passwords, 66

changing database server

How to, 38, 45

changing default administrator credentials

How to, 9

changing expiration duration of login key

m_setting table

How to, 62

changing the metadata database

How to, 45

changing user passwords

How to, 66

clearing

cache, 63

clearing the cache

How to, 64

clearing the cache by stopping aspnet process

How to, 64

client variables and business constants

understanding, 29

client-side log information

configuring, 74

compound controls

AgileTenKey, 13

configuration

users and groups, 74

configuring

business objects, 15

client-side log information, 74

conflict notification for sender and recipients, 75

history, 74

IIS authentication, 52

LDAP user authentication, 57

logging levels, 74

login method, 61

metrics collection, 74

Application Administrator tool

active directory

authentication, 56

Motorola Settings tool

SOAP authentication, 59

remote database, 40

users and groups, 65

configuring anonymous access

IIS server, 57

configuring conflict notification

How to, 75

configuring domain account, 40

configuring IIS directory security

How to, 53, 57

configuring logging levels

How to, 74

configuring login method authentication

How to, 62

configuring machine.config file

export resources

How to, 49

configuring metrics collection

How to, 74

configuring Application Administrator tool

LDAP Authentication, 58

configuring Application Administrator tool for active directory authentication

How to, 56

configuring Application Administrator tool for LDAP authentication

How to, 58

configuring Motorola Settings tool

How to, 55

IIS authentication, 55

SOAP authentication

How to, 59

configuring Motorola Settings tool to use Login Methos

How to, 62

configuring security

Application Administrator tool, 54

configuring SOAP/Active Directory authentication, 55

How to, 55

configuring SOAP/LDAP

user authentication, 57

conflict notification

configuring, 75

conflict resolution, 78

viewing, 78

connecting

metadata database

local, 35

remote, 39

controls

binding data, 13

create a business rule, 26

Create and Modify

Business Constants, 11

creating

business rule, 25

business rule resource, 23

configuring

domain account, 40

local user account, 54

users, 65

creating a Dexterra business object property

How to, 21

creating and configuring domain account

How to, 41

creating business object

How to, 16

creating local user account

How to, 54

creating security groups

How to, 69

creating users

How to, 65

credentials

Administrator

changing defaults, 9

D

data

binding, 13

exporting, 48

importing, 48, 49

data source authentication

methods, 52

database

configuring

remote, 40

metadata, 34

database server

changing, 45

changing, 38

define

business categories, 28

define a Dexterra business constant

How to, 28

defining

AgileTenKey compound controls, 13

AutoPersist property, 13

business object property

mapping business object properties to business objects, 20

business objects, 16

business rules, 25

business rules in the Application Administrator tool, 27

Edit property, 13

event generators, 33

terms, 3

defining a Dexterra business category

How to, 28

defining a Dexterra business object event and map it to a business rule

How to, 32

defining a Dexterra business rule

How to, 27

defining an event generator

How to, 33

deleting

users, 66

deleting a business object

How to, 22

deleting an existing business object property

How to, 22

deleting Dexterra business object

How to, 20

deleting users

How to, 66

denormalizing

business objects for better performance, 20

deploying

Motorola Application Server, 34

deployment

Motorola Application Server, 34

device

Smartphones, 5

Windows Mobile 2003 Second Edition, 5

Windows Mobile 5.0, 5

disable

permissions imported users and groups, 61

disable metric collection

Web method, 63

disabling

user permissions, 67

disabling metrics collection

How to, 74

disabling user permissions

How to, 67

disabling Web method

metric collection tool

How to, 63

distributed topologies

understanding, 40

documentation, 2

domain account

configuring, 40

E

Edit property

agile controls, 13

enabling

user permissions, 67

enabling history

How to, 74

enabling metrics collection

How to, 74

enabling SOAP authentication, 59

How to, 59

enabling user permissions

How to, 67

event generators

working with, 32

exporting data, 48

How to, 48

exporting logs to text file

How to, 76

exporting resources, 49

H

hardware requirements, 4

history

configuring, 74

viewing, 77

**How to**

add domain user

SQL Server database users, 41

add new business object to an application, 23

add sub-groups to security group, 70

add users to a groups, 72

assign .Net permissions, 41

assign permissions to security groups, 69

assign read and write permissions, 37

change database server, 38, 45

change default administrator credentials, 9

change expiration duration of login key

m_setting table, 62

change the account that runs Visual Studio .Net processes, 47

change the metadata database, 45

change user passwords, 66

clear the cache, 64

clear the cache by stopping aspnet process, 64

configure conflict notification, 75

configure IIS directory security, 53

configure IIS directory security, 57

configure logging, 74

configure login method authentication, 62

configure machine.config file

export resources, 49

configure metrics collection, 74

configure Application Administrator tool for active directory authentication, 56

configure Application Administrator tool for LDAP authentication, 58

configure Motorola Settings tool, 55

SOAP authentication, 59

configure Motorola Settings tool to use Login Method, 62

configure SOAP/Active Directory authentication, 55

create a business object, 16

create a Dexterra business object property, 21

create and configure domain account, 41

create local user accounts, 54

create security groups, 69

create users, 65

define a Dexterra business category, 28

define a Dexterra business constant, 28

define a Dexterra business object event and map it to a business rule, 32

define a Dexterra business rule, 27

define an event generator, 33

delete a business object, 22

delete an existing business object property, 22

delete Dexterra business object, 20

delete users, 66

disable metrics collection, 74

disable user permissions, 67

disable Web method

metric collection tool, 63

enable logging, 74

enable SOAP authentication, 59

enable user permissions, 67

export data, 48

export log to delimited text file, 76

import data, 49

import users and groups, 60

limit displayed records in a log, 76

log on to

metadata database, 38

log on to remote metadata database, 44

log on to the Application Administrator tool, 8

map a Dexterra business object property to a view column, 22

name an assembly in Application Administrator tool, 23

permanently delete log records, 76

remove a business object from an application, 24

remove a client table view from a business object, 19

remove an business object event definition, 32

remove sub-groups from a group, 71

remove users from groups, 73

run Visual Studio .Net process

domain user

running, 56

select the object value that will prevail, 78

sort log records, 76

verify ASPNET account permissions, 36

verify security settings, 54

view calls to user tables, 77

view conflict resolution, 78

view log records, 75

view metric data

associated with a web service, 77

I

identifying

account to run Visual Studio.Net process, 46

document scope, 2

supported devices, 5

Identifying

tasks of an administrator, developer, and analyst, 10

identifying installation prerequisites, 3

IIS authentication

configuring, 52

configuring Motorola Settings tool, 55

IIS directory security

configuring, 52

data source, 52

IIS Server

configuring

anonymous access, 57

implementing

security, 50

imported users and groups

disable permissions, 61

importing

users and groups, 60, 65

importing data, 48, 49

How to, 49

importing users and groups

How to, 60

initializing

logging on Client Application, 79

Initiating

Business Object Events, 31

installation prerequisites, 3

installations

single-server, 36

interpreting

web service web methods, 77

introduction, 1

invoking

business rules, 25

L

LDAP authentication

configuring

Application Administrator tool, 58

LDAP user authentication

configuring, 57

limiting displayed records in a log

How to, 76

local user account

creating, 54

log records

viewing, 75

loggin on to

metadata database

How to, 38

logging levels

configuring, 74

logging on to

metadata database, 38

Application Administrator tool, 8

logging on to a remote metadata database

How to, 44

logging on to remote metadata database, 44

logging on to the Application Administrator tool

How to, 8

login method

configuring, 61

Motorola Settings tool, 62

M

mapping a Dexterra business object property to a view column

How to, 22

metadata database, 34

account permissions, 36

changing, 44

connecting

local, 35

remote, 39

logging on to, 38

Motorola Application Server can connect

verifying, 37

naming conventions, 35

securing, 45

metric collection

Web method, 63

metrics

viewing Web Service Web methods, 77

metrics collection

configuring, 74

Application Administrator tool

accounts, 7

configuring security, 54

logging on to, 8

understanding, 7

user roles, 7

Motorola Application Server, 6

Motorola Settings tool

configuring, 55

login method, 62

configuring SOAP, 59

configuring SOAP authentication, 59

IIS authentication

configuring, 55

N

naming

your assembly in the Dexterra Conductor, 23

naming, 23

naming an assembly in Application Administrator tool

How to, 23

naming conventions

metadata database, 35

new business objects to your small factor application

adding, 23

P

permanently deleting log records

How to, 76

permissions

account

metadata database, 36

administrative

imported users and groups, 61

disable imported users and groups, 61

R

references, 2

removing

a client table view, 19

sub-groups from security groups, 71

users from groups, 73

removing a business object from an application

How to, 24

removing a client table from a business object

How to, 19

removing an business object event definition

How to, 32

removing sub-groups from a group

How to, 71

removing users from groups

How to, 73

requirements

hardware, 4

software, 4

requirements for Windows Server 2003

software, 4

requirements for Windows Server 2003 standard edition

software, 5

requirements for Windows XP Server

software, 4

resources

exporting, 49

using, 22

running .Net process

domain user

How to, 56

running Visual Studio.Net process

domain user

running, 56

S

saving

related objects when saving the business object, 20

saving the business object

saving related objects, 20

securing

metadata database, 45

user access to applications, 50

security

implementing, 50

security group, 69

sub-group

adding, 70

removing, 71

security groups, 68

assigning permissions, 69

selecting the object value that will prevail

How to, 78

server

architecture, 6

database

changing, 38

Simple Object Access Protocol, 3

single business

updating, 30

single-server

install, 36

installations, 36

installing, 36

SOAP, 3

SOAP authentication

enabling, 59

SOAP/Active Directory authentication

configuring, 55

SOAP/LDAP authentication

configuring, 57

software requirements, 4

software requirements for Windows Server 2003, 4

software requirements for Windows Server 2003 standard edition, 5

software requirements for Windows XP Server, 4

sorting log records

How to, 76

SSL, 3

synchronize business object method

using, 30

synchronizing

client variables and business constants, 29

T

TenKey

agile controls, 13

topologies

distributed, 40

U

UDDI, 3

understanding

business constants, 28

business object links, 20

business objects, 15

conflict notifications, 75

conflict resolution, 78

foreign keys, 20

Application Administrator tool, 7

one to one to many table column to table relationships, 21

synchronize business object method, 30

Universal Description, Discovery, and Integration, 3

updating

single business, 30

user access to applications

securing, 50

user account

local

creating, 54

user authentication

workflow, 51

user interface, 3

user passwords

changing, 66

user permissions

disabling, 67

enabling, 67

user roles

Application Administrator tool, 7

user status

verifying, 67

users

creating, 65

deleting, 66

users and groups

configuration, 74

configuring, 65

importing, 60, 65

users from group

removing, 73

users to group

adding, 72

using

resources, 22

SynchronizeApplication method to replace business constant value with a client
variable, 30

VS.NET to create a business rule, 26

V

verify security settings

How to, 54

verifying

Motorola Application Server can connect

metadata database, 37

Motorola Application Server connectivity to metadata database, 37

user status, 67

verifying ASPNET account permissions

How to, 36

view log information, 75

viewing

conflict resolution, 78

history, 77

log records, 75

Web service Web method metrics, 77

viewing calls to user tables

How to, 77

viewing conflict details

How to, 78

viewing log records

How to, 75

viewing metric data

associated with a web service

How to, 77

Visual Studio .Net process

running, 56

domain user, 56

Visual Studio.Net account

changing, 47

identifying, 46

W

Web method

metric collection tool, 63

Web Service Description Language, 3

web service web methods

interpreting, 77

Web Services, 3

working with

event generators, 32

WSDL, 3

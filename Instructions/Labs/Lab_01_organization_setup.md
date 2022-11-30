# Lab 01: Organization Setup

## Overview

### Background

In this lab for Microsoft Cloud for Sustainability you will build on top of demo data to configure the “Set up organization and reference data” scenario. Contoso Corp (*organization* *present in the demo data*) is a specialty Coffee distribution business with operations in APAC, US, Africa, and Europe.

Contoso Corp is experiencing Supply chain challenges to transport its finished goods across the USA and wants to augment its transportation and logistics capacities. To meet this challenge, Contoso Corp acquires a transportation business called Wide World Importers based in Florida, USA. Wide World Importers has two office facilities with 100 employees that coordinate a fleet of 40 electric trucks that will be used for transportation of finished goods across the USA.

### Learning Objectives

In this lab, you will perform the following:

- Review the company profile for Contoso Corp, add Wide World Importers to the organizational structure, and add the two Florida facilities

- Create reference data for contractual types

- Create units with conversion factor

- The newly created data during this lab exercise will form the foundation for the rest of the scenarios (data ingestion, calculations, and reporting) in the upcoming lab exercises.

### Prerequisites

- Microsoft Sustainability manager environment is set up with sample data

### Solution Focus Area

Organization setup focuses on the foundational steps required to configure the Microsoft Sustainability Manager application. These foundational steps will create the company profile, set up organizational structure and hierarchy, and corresponding facilities. After this, reference data will be set up that includes important information such as fuel types, vehicle types, contractual instrument types, and units. Some of this reference data is unique to an organization, and some will come from standard or industry sources.

![Diagram Description automatically generated](./Images/Lab01/L01_image001.png)

### Personas and Scenarios

In this lab, Jessie Irwin – Sustainability lead for Contoso Corp and Amber Rodriguez - Sustainability Specialist for Contoso Corp educate Alex Serra of Wide World importers on the tools and processes used for Contoso’s Sustainability reporting. Jessie guides Alex to build an inventory management plan by listing out the operating boundaries, facilities, and emission sources. Jessie and Amber demonstrate “Microsoft Sustainability Manager” and share the inventory plan template with Alex Serra – Emissions Analyst and Reed Flores – IT Admin. After completing the Inventory plan template - together, Alex and Reed set up the Company Profile, Organization data and Reference data based on the data provided by Amber in the Inventory plan.

![Diagram Description automatically generated](./Images/Lab01/L01_image002.png)

In this lab exercise, we will focus on the scenarios illustrated below:

![](./Images/Lab01/L01_image003.png)

## Exercise 1: Set up company profile and reference data

In this exercise, you will learn about the steps that Alex and Reed take to set up Wide World Imports company profile, organizational data, and reference data. You can explore this functionality in deeper detail on Microsoft Docs, please visit [Set up a company profile](https://docs.microsoft.com/en-us/industry/sustainability/setup-company-profile).

-   For our Instructor Lead Training, we suggest using In-private browsing, or a new browser profile.
-   For our Instructor Lead Training, log in to <https://make.powerapps.com> using the mcfsiaduserXX@powerplatformopenhacks.onmicrosoft.com account that has been assigned to you.
-   For our Instructor Lead Training, please use the environment selector to select the MCFSInADay_XX environment that has been assigned to you

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image004.png)

-   Open the **Sustainability Manager** Application

    ![Graphical user interface, application, Teams Description automatically generated](./Images/Lab01/L01_image005.png)

You will land on the **Home** page for Microsoft Sustainability Manager

![A screenshot of a computer Description automatically generated](./Images/Lab01/L01_image006.png)

 >[!NOTE]**Note**: You can dismiss the Product tour by scrolling down and clicking on the “Dismiss tour” button.

 ![Graphical user interface, text, application Description automatically generated](./Images/Lab01/L01_image007.png)

Area navigation is a common first step in each lab and exercise. You can find the area navigation menu in the bottom corner of your screen.

![](./Images/Lab01/L01_image008.png)

## Task 1: Setup the Company profile, hierarchy, and facilities

In this task, Alex sets up the Company profile, hierarchy, and facilities for the Wide World Importers organization in Microsoft Sustainability Manager.

1. In the bottom left corner, change your Area to **Settings**

    ![](./Images/Lab01/L01_image009.png)

1. Navigate to “**Company profile**” on the left side of the page.

    ![](./Images/Lab01/L01_image010.png)

1. The Company profile page includes basic information about the organization, such as name, address, company logo, the annual reporting period, and relevant industries. Additionally, there are tabs at the top of the page for setting up organization structure and facilities, both will be covered in this exercise.

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image011.png)

1. On the **Company profile** page, Click on **Industries** Tab. Microsoft Sustainability Manager includes a selection of pre-defined industries and sub-verticals based on NACE standards, [NACE Code](https://nacev2.com/en). Click +**Add**

    ![](./Images/Lab01/L01_image012.png)

1. In the **Industries** section select **Transportation and storage**

    ![Graphical user interface, application, PowerPoint Description automatically generated](./Images/Lab01/L01_image013.png)

1. In the next screen select **“Land transport and transport via pipelines”** and select **“Add”**

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image014.png)

1. “**Land transport and transport via pipelines**” is now visible in the Industries section at the bottom of the **Company profile** page

    ![Graphical user interface, website Description automatically generated](./Images/Lab01/L01_image015.png)

1. In the **Company profile** page switch to the **Structure** tab

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image016.png)

1. Select **Contoso USA** and select **Add** to add a new organizational unit under it.

    ![Graphical user interface, application, table Description automatically generated](./Images/Lab01/L01_image017.png)

1. Enter the following data for organizational unit and select **Save** in the button pane

    - **Name**: Wide World Importers

    - **Organizational unit type**: Department

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image018.png)

1. In the Organizational hierarchies section, which appears after clicking **Save**, click + **New Organizational hierarchy**

    ![Graphical user interface, text, application, email Description automatically generated](./Images/Lab01/L01_image019.png)

1. Set the following values and click **Save & Close**

    - **Parent**: Contoso USA

    - **Effective start date**: The first day of the current month (MM/DD/YYYY)

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image020.png)

1. After being returned to the Organizational Unit, click **Save & Close** to return to the **Company profile**

    ![Graphical user interface, text, application, email Description automatically generated](./Images/Lab01/L01_image021.png)

1. Navigate to **Company profile** switch to **Facilities** tab page and select **Add facility**

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image022.png)

1. Create a new Facility with the following details. Once the values are entered, select **Save & Close**

    >[!NOTE] **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

    - **Name**: Wide World Importers - Miami Office

    - **Address line 1**: Brickell Avenue

    - **City**: Miami

    - **State**: Florida

    - **Zip**: 33132

    - **Country**: United states of America

    - **Latitude**: 25.774320

    - **Longitude**: -80.187720

    >[!NOTE] **Note:** Latitude and Longitude are not required but are used to display a pin on the Facilities map. They can be automatically added by selecting an address from the autocomplete options in Address line 1, or manually entered.

![](./Images/Lab01/L01_image023.png)

1. Using the same steps, add another new **Facility**. Once the values are entered, select **Save & Close**

    >[!NOTE] **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

    - **Name**: Wide World Importers - Tampa Office

    - **Address line 1**: Lois Avenue

    - **City**: Tampa

    - **State**: Florida

    - **Zip**: 33609

    - **Country**: United states of America

    - **Latitude**: 27.944830

    - **Longitude**: -82.514050

    >[!NOTE] **Note:** Latitude and Longitude are not required but are used to display a pin on the Facilities map. They can be automatically added by selecting an address from the autocomplete options in Address line 1, or manually entered.

![](./Images/Lab01/L01_image024.png)

Great job, by completing these steps, you have completed the organizational setup. Organizational structure and facility management will be linked to activity and emission data to group emissions by Organization, facility, and even regions. This is an important part of carbon emission reporting and organization disclosures. **Please continue to the next task.**

## Task 2: Setup reference data

In this task, Reed sets up the reference data for contractual instrument types in Microsoft Sustainability Manager. Contractual instrument types are the different types of contractual agreements that a firm has with their providers and suppliers.

1. In the bottom left corner, change the Area to **Settings**

    ![Graphical user interface, application Description automatically generated](./Images/Lab01/L01_image025.png)

1. Navigate to “**Reference data**” on the left side of the page.

    ![](./Images/Lab01/L01_image026.png)

1. Select **Contractual instrument types** and select **View**

    ![Graphical user interface, text, application Description automatically generated](./Images/Lab01/L01_image027.png)

1. Under **Active contractual instrument types \>Select New** to create new contractual types

    ![Graphical user interface, text, table Description automatically generated with medium confidence](./Images/Lab01/L01_image028.png)

1. Create a new Contractual Instrument with the following details. Once entered, select **Save & Close** in the button pane.

    - **Name**: VanArsdel Ltd

    - **Energy source**: Nuclear

    >[!NOTE] **Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

    ![](./Images/Lab01/L01_image029.png)

    >[!NOTE]**Note:** Pay close attention to the data used in this lab. The following labs will reference this data, and it will need to match exactly as seen in the lab.

1. In the same way, again create a new Contractual Instrument with the following details. Once entered, select **Save & Close** in the button pane.

    - **Name**: Adatum Corp

    - **Energy source**: Other

    ![](./Images/Lab01/L01_image030.png)

Great job, by completing these steps, you have added contractual instrument types. There are many types of reference data, take some time after this lab to explore the other reference data types, they will be used throughout Microsoft Cloud for Sustainability, and Microsoft Sustainability Manager. **Please continue to the next task.**
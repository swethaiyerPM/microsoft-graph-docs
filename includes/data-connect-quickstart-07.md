---
ms.localizationpriority: medium
---

## Visualize your Graph Data Connect data in PowerBI

This exercise describes how to create a report in PowerBI to visualize your Microsoft 365 data from Microsoft Graph Data Connect.

As a pre-requisite, you need to complete the steps in this tutorial. Once you have your JSON file in your Azure Storage complete the following steps:

1. Open your PowerBI desktop application or download it from: [Download Power BI tools and apps](https://powerbi.microsoft.com/en-us/downloads/)  

2. Click on the **Get Data** window, select **Azure** and choose **Azure Blob Storage** from the list of Azure services.

3. Click **Connect** to establish the connection between Power BI and your Azure Blob Storage account.

![A screenshot that shows how to connect to get data from an Azure Blob Storage in PowerBI](../concepts/images/data-connect-pbi-connect-blob-storage.png)

4. **Add the Azure Blob Storage Account name or URL:** enter the Storage Account name and container name for the Azure Blob Storage account you want to connect to, then click **OK**.

![A screenshot that shows how to add the Azure Blob Storage account URL to get data in PowerBI](../concepts/images/data-connect-pbi-add-blob-account-name.png)

> **Note** You can find your Azure Storage URL in the Azure storage account, go to your containers and choose the container you would like to connect, click on the Context menu (...) select **Container properties** and copy the URL.  

5. Select **Transform Data** and click to go inside the first line that says **Binary**.

![A screenshot that shows how to transform the binary data in PowerBI](../concepts/images/data-connect-pbi-transform-binary.png)

6. On the Column1 toggle option, right click to select **Transform** then choose **JSON**. You will get a list with all the **Records**.

![A screenshot that shows how to expand the data columns in PowerBI](../concepts/images/data-connect-pbi-transform-columns.png)

7. Expand the **Records** from the Column1 toggle, it will load all the columns, then click **OK**.

![A screenshot that shows how to load all the columns in PowerBI](../concepts/images/data-connect-pbi-expand-records.png)

6. The results will be shown as (Column1.property), you can now expand again the columns with nested data by clicking on the toggle option on each column, then click **OK**.

    - You can now click on **Close & Apply** and wait for your query to load all the columns.

    ![A screenshot that shows how to load all the columns in PowerBI](../concepts/images/data-connect-pbi-expand-columns-close.png)

7. Once it loaded all the columns, you can now build visuals with your data.

    - Under **Data**, select Query1 to expand the columns and choose the properties you would like to visualize.
    - Under **Visualizations**, select the **Key Influencers** option to visualize the data.
    
> **Note** In this example you can easily see if the messages sent by a department in your organization are being read or not by analyzing every "toRecipientName" and the property "isRead".

![A screenshot that shows all the columns with content presented in a table in PowerBI](../concepts/images/data-connect-pbi-key-influencers.png)

8. We can now see the JSON data from the Messages_v1 data set from Microsoft Graph Data Connect in a PowerBI report.

> [!NOTE]
> You can choose the desired data connectivity mode (DirectQuery or Import) depending on your data size and query requirements. We recommend using **DirectQuery** in this tutorial.

 [Find solution templates using MGDC built in PowerBI](https://github.com/microsoftgraph/dataconnect-solutions/tree/main/solutions)

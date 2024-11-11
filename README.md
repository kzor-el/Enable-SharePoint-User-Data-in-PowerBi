# Enable-SharePoint-User-Data-in-PowerBi
How to create a relationship between user id to show details in Power BI

Follow the below steps to make a realtionship between SharePoint User ID and display their details in PowerBi (i.e. Display Name):
Fron PowerBI desktop:
1. Connect to SharePoint online lists via GetData - SharePoint online list url = "http://<mySharePointSite>/sites/sitename/"
2. Conenct to the User Information List in SharePoint via OData from PowerBI "GEtData-OData feed" to access the information url="http://<mySharePointSite>/_vit_bin/listdata.svc" then select "UserInformationList"
3. From mange realtion icon make relation between teh SharePoint task table "AssignToID" and UserInformationList"ID"
4. From edit query icon  select your SharePoint online task table and edit your AuthorIdEditorIdOData column by clicking on the small icon in the column header and select "expand to new rows" option then click close & apply.
5. Once you return PowerBI desktop chose Title from the "Sharepoint list" and Name from the "UserInformationList"

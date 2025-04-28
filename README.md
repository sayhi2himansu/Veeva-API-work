# Veeva API Python scripting to download viewable rendition in Bulk.

### Need of this script, WHY?
In veeva vault Renditions refer to the pdf version of the uploaded file but it doesn't include the signature rendition. Viewable rendition option downloads the PDF file including the signature rendition at the end or start of the document based on vault configurations. This option is available on the UI to manually downalod the viewable rendition but when the case is to download bulk Viewable Renditions during the migration activity - then there's a need to code.


### General tips for this script before execution
1. Pyhton scripting has been executed on the Jupiter notebook. One can get help of this script and use it in other coding tools as well.
2. Script  also generate the log file to identify if for amy doc ids - Code failed to download the viewable rendition.
3. "Credentials.txt" file contains the Vault environment URL and the veeva API version. One can use the latest version of API by editing the "credentials.txt" file.
4. Script contains your session IDs for vault authentication(Basis Security policy). USE your test environment before the PROD executions.
5. For bulk downloading the Viewable Renditions - One will have the CSV file with DOC IDs. Script will read the ID from this CSV and using API GET method download the content.

   


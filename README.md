# ETL-Project
This is the repository for the group project of ETL Data Warehousing class at DSTI.
## Repository Contents

- **Source data files**
- **SQL queries for table creation**
- **STA, ODS, DWH packages**
- **Project Report**

## Guidelines for Reproduction

To run the project, please follow these steps:

1. **Install Prerequisites**:
    - Install [Visual Studio Community 17.9.7](https://visualstudio.microsoft.com/vs/community/) or higher, with the SSDT (SQL Server Data Tools) package.
    - Add the SSIS extension to Visual Studio.

2. **Setup SQL Server**:
    - Create a local SQL server and use an alias called "ServiceSpot" for the server. Follow the instructions in this [YouTube video](https://www.youtube.com/watch?v=PaRFj-uzLhc&ab_channel=AllTech).

3. **Create Databases**:
    - Create four databases in SQL Server: `SS_ADM`, `SS_STA`, `SS_ODS`, `SS_DWH`.

4. **Clone the Repository**:
    - Clone this repository using Visual Studio or your preferred Git tool.

5. **Modify Packages**:
    - Update the following packages to include the paths to the CSV source data files (by default, they are set to the Administrator folder):
        - `ProjectParams`
        - `STA_Data` (located in the FELC container)

6. **Run ETL Pipeline**:
    - Execute the `ETL-Pipeline` package. This will:
        - Create all necessary tables using T-SQL.
        - Launch all the STA, ODS, and DWH packages.

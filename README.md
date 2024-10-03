# PLSQL-Assignment
## Tasks Completed

1. Created a Pluggable Database (PDB) named `plsql_class2024db`.
2. Created and deleted a PDB named `is_to_delete_pdb`.
3. Configured Oracle Enterprise Manager (OEM).
1.
## SQL Queries Used

### 1. Create PDB `plsql_class2024db`
```sql
CREATE PLUGGABLE DATABASE plsql_class2024db 
ADMIN USER plsql_class2024db IDENTIFIED BY snakie05 
FILE_NAME_CONVERT = ('C:\APP\USER\ORADATA\ORCL\PDBSEED\', 'C:\APP\USER\ORADATA\ORCL\PDB\');
2.
CREATE PLUGGABLE DATABASE is_to_delete_pdb 
ADMIN USER is_plsqlauca IDENTIFIED BY your_password 
FILE_NAME_CONVERT = ('C:\APP\USER\ORADATA\ORCL\PDBSEED\', 'C:\APP\USER\ORADATA\ORCL\PDB\is_to_delete_pdb\');
3.
DROP PLUGGABLE DATABASE is_to_delete_pdb INCLUDING DATAFILES;

# Banking-Management-System

### How to Restore the Database

1. Download the `.bak` file from this repository.
2. Open SQL Server Management Studio (SSMS).
3. Run the following SQL command to restore the database:
   ```sql
   RESTORE DATABASE BankingSystem
   FROM DISK = 'C:\Program Files\Microsoft SQL Server\MSSQL16.SQLEXPRESS\MSSQL\Backup\BankingSystem.bak'
   WITH MOVE 'BankingSystem_Data' TO 'C:\Program Files\Microsoft SQL Server\MSSQL16.SQLEXPRESS\MSSQL\Data\BankingSystem.mdf',
        MOVE 'BankingSystem_Log' TO 'C:\Program Files\Microsoft SQL Server\MSSQL16.SQLEXPRESS\MSSQL\Data\BankingSystem.ldf';

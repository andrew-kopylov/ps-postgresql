# ps-postgresql
Powershell module for PostgreSQL

Functions
- Backuping
  Invoke-PgBackup($DbName, $BackupDir, $Period = "", [int]$StorePeriods = 0, $Srvr = $null, $Port = $null) - create backups
    - DbName - String - db's name for backuping
    - BackupDir - String - full path of directory for backup file
    - Period - String (optional) - values 'd' - day, 'w' - week, 'm' - month, 'y' - year
    - StorePeriod - int (optional) - count of storing periods
    - Srvr - String (optional) - pg server name (localhost)
    - Port - String (optional) - pg server port (5432)
    
  Remove-PgBackups($BackupDir) - remove packups files from directory with ended storing period.
  


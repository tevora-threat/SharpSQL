# sharpsql
Quick and dirty .net console app for querying mssql servers.

If you get an error like "Invoke Failed 3" or similar, you likely don't have proper permissions or your connection string is messed up. 

Usage: `SharpSQL.exe <Command> -ConnectionString <string>`

Commands: 
```
Query  Executes arbitrary query against the server using the provided connection string. Use this to select tables, xpcommandshell,etc
Usage: SharpSQL.exe Query -Query <query> -ConnectionString <string>

Check-DBAccess - Lists all databases your current user has access to
Usage: SharpSQL.exe Check-DBAccesss -ConnectionString <string>


Get-Databases - Lists all databases on the server
Usage: SharpSQL.exe Get-Databases -ConnectionString <string>

Get-Tables - Lists all tables in current database. Database is set in connection string. 
Usage: SharpSQL.exe Get-Tables -ConnectionString <string>

Check-CurrentDBPerms - Enumerates permissions for current database. Database is set in connection string. 
Usage: SharpSQL.exe Check-CurrentDBPerms -ConnectionString <string>
```

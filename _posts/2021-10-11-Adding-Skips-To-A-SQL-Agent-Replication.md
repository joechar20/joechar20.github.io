## Adding Skips to a SQL Agent replication distribution job

#### This covers a basic example of adding skips to a SQL Server Transactional Replication Distribution job, by editing the job steps. 
#### Pre-requisites: Familiarity with SQL Server Agent jobs. Monitoring with the SQL Agent Job Activity monitor and editing steps using the job properties.

Step 1: Identify the job(s) with a category of "REPL-Distibution" using the SQL Agent Job Activity monitor
https://imgur.com/a/A6IFIQR
### This is a header

#### Some T-SQL Code

```tsql
SELECT This, [Is], A, Code, Block -- Using SSMS style syntax highlighting
    , REVERSE('abc')
FROM dbo.SomeTable s
    CROSS JOIN dbo.OtherTable o;
```

#### Some PowerShell Code

```powershell
Write-Host "This is a powershell Code block";

# There are many other languages you can use, but the style has to be loaded first

ForEach ($thing in $things) {
    Write-Output "It highlights it using the GitHub style"
}
```

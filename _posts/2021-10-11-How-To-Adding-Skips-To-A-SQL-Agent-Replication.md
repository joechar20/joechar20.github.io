## How To: Adding Skips to a SQL Agent replication distribution job

### This covers a basic example of adding skips to a SQL Server Transactional Replication Distribution job, by editing the job steps. 
#### Pre-requisites: Familiarity with SQL Server Agent jobs. Monitoring with the SQL Agent Job Activity monitor and editing steps using the job properties.
#### Pre-requisites: Familiarity with SQL Server Agent jobs. Monitoring with the SQL Agent Job Activity monitor and editing steps using the job properties.

Step 1: Identify the job(s) with a category of "REPL-Distibution" using the SQL Agent Job Activity monitor
![SQL Agent Job Activity Monitor Category](https://github.com/joechar20/joechar20.github.io/blob/main/_Images/2021-10-11/ActivityMonitorCategory.png?raw=true)

Step 2: Open the job properties -> Steps -> (select step) “Run agent.” -> click “Edit”
![Replication Distribution Job properties](https://github.com/joechar20/joechar20.github.io/blob/main/_Images/2021-10-11/JobProperties.png?raw=true)

Step 3: Scroll all the way to the right of the text and after the last parameter you will add the skips
“-SkipErrors 2601:2627:20598”
![Job Step Properties adding skips](https://github.com/joechar20/joechar20.github.io/blob/main/_Images/2021-10-11/JobStepProperties_AddingSkip.png?raw=true)

Step 4: Click OK -> Click OK
Step 5: Stop and start the job you just updated so the new parameters are used.

Note: to remove the skips you can remove them from the job and re-start it.

### Microsoft Documentation links

Skipping Errors in Transactional Replication: https://docs.microsoft.com/en-us/previous-versions/sql/sql-server-2008-r2/ms151331(v=sql.105)

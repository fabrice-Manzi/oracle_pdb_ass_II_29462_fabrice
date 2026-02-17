# MANZI FABRICE
# ID:29462
# ASSIGNMENT II: ORACLE PLUGGABLE DATABASE (PDB) MANAGEMENT

## TASK OVERVIEW
This assignment was mainly focusing on** Oracle Multitenant Architecture**. Mainly on creation and deletion of pluggable database(PDB), user creation and management inside a PDB, use of oracle enterprise manager(OEM) and technical documentation using GitHub. 
** Oracle Environment** 
In this assignment, I used **oracle 21c** which has built-in feature of OEM.

## TASKS BREAKDOWN
I worked on 3 main tasks in this assignment.
### TASK1: Creation of new pluggable database(PDB).
As the screenshot below illustrate, I created a new pluggable database named **fa_pdb_29462** and then opened it.
- ![PDB CREATION SCREENSHOT](pdb-created-successfully.png)
- ![PDB OPEN STATUS SCREENSHOT](pdb-mode-status.png)
  
After the creation of new PDB, I created a user inside that PDB with username of **fabrice_plsqlauca_29462** and granted all privileges on the PDB. the next screenshot shows the commands for the user creation in sql*plus.
- ![USER CREATION SCREENSHOT](user-created.png)
  
#### COMMANDS USED
- PDB Creation:**create a pluggable database fa_pdb_29462 admin user pdbadmin identified by manzi004# file_name_convert('c:\app', 'c:\app');**
- PDB Open State: **alter pluggable database fa_pdb_29462 open;**
- PDB User Creation: **create user fabrice_plsqlauca_29462 identified by manzi004#;**

### TASK2: create and delete a PDB.
Here I created another temporary PDB named as **fa_to_delete_pdb_29462** and then later deleted it. The screenshot below shows the PDB created successfully and then deleted.
- ![TEMPORARY PDB CREATION SCREENSHOT](temporary-pdb-creation.png)
- ![PDB DELETION SCREENSHOT](deletion-command.png)
- 
#### COMMANDS USED
- PDB Creation:**create a pluggable database fa_to_delete_pdb_29462 admin user pdbadmin identified by manzi004# file_name_convert('c:\app', 'c:\app');**
- PDB Open State: **alter pluggable database fa_to_delete_pdb_29462 open;**
- PDB deletion: **drop pluggable database fa_to_delete_pdb_29462 including datafiles;**

### TASK3: Oracle Enterprise Manager (OEM).
From this task I have accessed the OEM dashboard as my user in PDB level as shown in the below screenshot.
- ![OEM DASHBOARD SCREENSHOT](MANZI-OEM-DASH.png)
- OEM LINK: <https://localhost:5510/em>

## CHALLENGES 
During the time of doing this assignment the challenges i faced include:
- **I didn't know sql commands to use**: to overcome this I used some youtube videos to see more about use of pl/sql commands as well using our notes and other AI tools to help understand it clearly the commands used.
- **Installation of oracle 21c**: this was among the first challenge i faced where these was failed due to not enough memory to create a database. So I installed software only and then using database configuration assistant I managed to create a database later.
- **Access to OEM as PDB user**: this was another challenge that i faced where i was only accessing OEM as only sys user.

## INTEGRITY STATEMENT
I declare that this repository contains my original work done independently. I haave not copied or used unauthorized materials from any other person or source.

### IN SUMMARY
this assignment have left me with some pratical skills on oracle multitenant architecture and GitHub basic skills for documentation.

## COMMANDS USED IN ASSIGNMENT
- PDB Creation:**create a pluggable database PDB_NAME admin user pdbadmin identified by PASSWORD# file_name_convert('c:\app', 'c:\app');**
- PDB Open State: **alter pluggable database PDB_NAME open;**
- PDB User Creation: **create user USERNAME identified by PASSWORD;**
- PDB deletion: **drop pluggable database fa_to_delete_pdb_29462 including datafiles;**
- PDBs Availble: **show pdbs**
- Changing session/container: **alter session set container=con_name**
- see container name: **show con_name**
- link to access OEM:<https://localhost:5510/em>

  # FINAL ASSIGNMENT CHECKLIST
- [v] Create PDB names used
- [v] User created inside the PDB
- [v] Temporary PDB created and deleted
- [v] OEM Dashboard screenshot included
- [v] GitHhub repository is public
- [v] READMEcis clear and professional
- [v] Deadline respected

   - **Reposiory link**:<https://github.com/fabrice-Manzi/oracle_pdb_ass_II_29462_fabrice>
  - PDB NAME CREATED: FA_PDB_29462
  - ISSUES ENCOUNTERED: [YES]
    
-------------------------------------------------------THANK YOU------------------------------------------------------------




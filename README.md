# ASSIGNMENT II: ORACLE PLUGGABLE DATABASE (PDB) MANAGEMENT
## TASK OVERVIEW
This assignment was mainly focusing on** Oracle Multitenant Architecture**. Mainly on creation and deletion of pluggable database(PDB), user creation and management inside a PDB, use of oracle enterprise manager(OEM) and technical documentation using GitHub. 
** Oracle Environment** 
In this assignment, I used **oracle 21c** which has built-in feature of OEM.
## TASKS BREAKDOWN
I worked on 3 main tasks in this assignment.
### TASK1: Creation of new pluggable database(PDB).
As the screenshot below illustrate, i created a new pluggable database named **fa_pdb_29462** and then opened it.
--------------------------------
After the creation of new PDB, I created a user inside that PDB with username of **fabrice_plsqlauca_29462** and granted all privileges on the PDB. the next screenshot shows the commands for the user creation in sql*plus.
--------------------------------
#### COMMANDS USED
. PDB Creation:**create a pluggable database fa_pdb_29462 admin user pdbadmin identified by manzi004# file_name_convert('c:\app', 'c:\app');**
. PDB Open State: **alter pluggable database fa_pdb_29462 open;**
. PDB User Creation: **create user fabrice_plsqlauca_29462 identified by manzi004#;**

### TASK2: create and delete a PDB.
Here i created another temporary PDB named as **fa_to_delete_pdb_29462** and then later deleted it. The screenshot below shows the PDB created successfully and then deleted.
-----------
#### COMMANDS USED
. PDB Creation:**create a pluggable database fa_to_delete_pdb_29462 admin user pdbadmin identified by manzi004# file_name_convert('c:\app', 'c:\app');**
. PDB Open State: **alter pluggable database fa_to_delete_pdb_29462 open;**
. PDB deletion: **drop pluggable database fa_to_delete_pdb_29462 including datafiles;**

### TASK3: Oracle Enterprise Manager (OEM).
From this task i have accessed the OEM dashboard as sys user in CDB level as shown in the below screenshot.
--------------------
OEM LINK: <https://localhost:5500/em>

## CHALLENGES 
During the time of doing this assignment the challenges i faced include:
1.** I didn't know sql commands to use**: to overcome this I used some youtube videos to see more about use of pl/sql commands as well using our notes and other AI tools to help understand it clearly the commands used.
2. ** Installation of oracle 21c**: this was among the first challenge i faced where these was failed due to not enough memory to create a database. So I installed software only and then using database configuration assistant I managed to create a database later.
3. **Access to OEM as PDB user**: this was another challenge that i faced where i was only accessing OEM as only sys user.

## INTEGRITY STATEMENT
--------------------------------
### IN SUMMARY
this assignment have left me with some pratical skills on oracle multitenant architecture and GitHub basic skills for documentation.
## COMMANDS USED IN ASSIGNMENT
. PDB Creation:**create a pluggable database PDB_NAME admin user pdbadmin identified by PASSWORD# file_name_convert('c:\app', 'c:\app');**
. PDB Open State: **alter pluggable database PDB_NAME open;**
. PDB User Creation: **create user USERNAME identified by PASSWORD;**
. PDB deletion: **drop pluggable database fa_to_delete_pdb_29462 including datafiles;**
. PDBs Availble: **show pdbs**
. Changing session/container: **alter session set container=con_name**
. see container name: **show con_name**
. link to access OEM:<https://localhost:5500/em>

## SCREENSHOT FOLDERS




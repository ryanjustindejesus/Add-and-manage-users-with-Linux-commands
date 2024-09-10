<h1>Adding and managing users with Linux commands </h1>



<h2>Description</h2>
In this lab, I learned how to add users and manage user access in a system. These skills can be used when working with authentication technology
<br />


<h2>Practical experience gained in this Lab</h2>

- <b>Adding a new user</b> 
- <b>Adding a user to a group</b>
- <b>Changing user permissions on files</b> 
- <b>Deleting a user</b> 

<h2>Environments Used </h2>

- <b>Qwiklabs</b> 

<h2>Lab walk-through:</h2>

<h2>Task 1: Description </h2>
A new employee has joined the Research department. In this task, I added them to the system. The username assigned to them is researcher9.
 <br/> <br />
(1) First, I used the command "sudo useradd researcher9" to add a user called researcher9 to the system. <br/> <br/>
(2) Then, I used the command "sudo usermod -g research_team researcher9" to add the new user, researcher9, to the research_team group. <br/> <br/>
(3) Finally, I used the command "id researcher9" to confirm that researcher9 has been added to the system. 
<br/> <br/> <p align="center">
<img src="https://imgur.com/H0MKixi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 2: Description </h2>
The new employee, researcher9, will take responsibility for project_r. In this task, I made them the owner of the project_r.txt file.
<br/> <br />
(1) First, I used the command "sudo chown researcher9 /home/researcher2/projects/project_r.txt" to make researcher9 the owner of the /home/researcher2/projects/project_r.txt. <br /> <br/>
(2) Finally, I used the command "ls -l /home/researcher2/projects/project_r.txt" to confirm that researcher9 is the owner of the project_r.txt file. 
<br /> <br /> <p align="center">
<img src="https://imgur.com/PPkgKSv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 3: Description </h2>
A couple of months later, this employee's role at the organization has changed, and they are working in both the Research and the Sales departments. In this task, I added 'researcher9' to a secondary group ('sales_team'). Their primary group is still `researcher_team'.
 <br/> <br/>
(1) First, I used the command "sudo usermod -a -G sales_team researcher9" to add researcher9 to the sales_team group as a secondary group. <br/> <br/>
(2) Finally, I used the command "groups researcher9" to confirm that researcher9 has been added to the secondary group, sales_team.
<br/> <br/> <p align="center">
<img src="https://imgur.com/r3kDpq3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

<h2>Task 4: Description </h2>
A year later, researcher9, decided to leave the company. In this task, I removed them from the system.
 <br/> <br/> 
(1) First, I used the command "sudo userdel researcher9" to delete researcher9 from the system. <br/> <br/>
(2) Finally, I used the command "sudo groupdel researcher9" to delete the researcher9 group that is no longer required. 
<br/> <br/>  <p align="center">
<img src="https://imgur.com/gfIl23P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<br /> <br />

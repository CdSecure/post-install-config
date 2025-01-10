<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
As the next step in setting up osTicket, this lab walks through the necessary changes to configure it into a fully functional ticketing system.
<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Configuration Steps</h2>

**Configuring osTicket as a Ticketing System**

After installing osTicket, follow these steps to configure it effectively as a ticketing system:

1. **Identify the Active Panel**
   - **Understand Panel Roles:**
     - osTicket features two distinct panels: **Admin Panel** and **Agent Panel**, each requiring different configurations.
   - **Determine the Active Panel:**
     - Look at the top right corner of the osTicket interface.
     - If it displays **"Agent Panel"**, you are currently in the Admin Panel.
     - Conversely, if it displays **"Admin Panel"**, the Agent Panel is active.

2. **Create a New Role: "Supreme Admin"**
   - **Access the Admin Panel:**
     - Ensure you are in the Admin Panel by verifying the panel name in the top right corner.
   - **Navigate to the Agents Menu:**
     - In the Admin Panel, click on the **Agents** menu.
   - **Create the "Supreme Admin" Role:**
     - Click on **Roles** within the Agents menu.
     - Select the option to **Create New Role**.
     - Enter **"Supreme Admin"** as the role name.
     - **Assign Permissions:**
       - For the purposes of this lab, assign **all available permissions** to the "Supreme Admin" role to grant comprehensive administrative capabilities.
   - **Save the New Role:**
     - Click **Save** or **Create** to finalize the role creation.
<p>
<img width="1800" alt="Screenshot 2024-12-09 at 3 49 58 PM" src="https://github.com/user-attachments/assets/c71c0d64-755c-40d2-8da9-c4f059651bd3">
<img width="1800" alt="Screenshot 2024-12-09 at 3 56 03 PM" src="https://github.com/user-attachments/assets/ca542de5-6362-429a-826a-12e6db950658">
</p>

**Creating a New Department for System Administrators in osTicket**

To establish a dedicated Department for System Administrators within osTicket, follow these professional steps:

1. **Access the Admin Panel**
   - Log in to the osTicket **Admin Panel** using your administrative credentials.

2. **Navigate to the Agents Menu**
   - In the Admin Panel, locate and click on the **Agents** menu to access agent-related settings.

3. **Open the Departments Section**
   - Within the Agents menu, select **Departments** to view and manage existing departments.

4. **Create a New Department**
   - Click on the **Add Department** button.
   - Enter **System Administrators** as the **Department Name**.
   - Configure any additional settings as required, such as assigning default email addresses or associating specific groups.

5. **Save the New Department**
   - After entering the necessary information, click **Save** or **Create** to finalize the creation of the **System Administrators** department.

<p>
<img width="1800" alt="Screenshot 2024-12-09 at 4 04 58 PM" src="https://github.com/user-attachments/assets/c42957f5-d4ec-4a71-a90f-4c8e64d783fa">
</p>

**Creating a Level II Support Team in osTicket**

To enhance support capabilities, we will create a new Level II Support Team to complement the existing Level I Support Team within osTicket. Follow the steps below to set up the Level II Support Team effectively.

### **Steps:**

1. **Access the Admin Panel**
   - **Log In:**
     - Open your web browser and navigate to your osTicket installation.
     - Enter your administrative credentials to log into the **Admin Panel**.

2. **Navigate to the Agents Menu**
   - **Open Agents Settings:**
     - In the Admin Panel, locate and click on the **Agents** menu. This section manages all agent-related configurations.

3. **Open the Teams Section**
   - **Access Teams Management:**
     - Within the Agents menu, select **Teams**. This will display a list of existing support teams.

4. **Create a New Level II Support Team**
   - **Add New Team:**
     - Click on the **Add Team** button to initiate the creation of a new support team.
   - **Configure Team Details:**
     - **Team Name:** Enter **"Level II Support"** as the team name.
     - **Description:** Optionally, provide a description outlining the responsibilities and scope of the Level II Support Team.
     - **Assign Departments:** Associate the team with relevant departments (e.g., **System Administrators**) to ensure proper ticket routing.
     - **Set Permissions:** Define the permissions and access levels for team members to manage tickets effectively.
   - **Save the Team:**
     - After configuring the details, click **Save** or **Create** to finalize the creation of the **Level II Support** team.

5. **Assign Agents to the Level II Support Team**
   - **Select Team Members:**
     - Navigate to the **Agents** section within the **Teams** menu.
     - Select the **Level II Support** team and click on **Manage Agents**.
   - **Add Agents:**
     - Choose the agents who will be part of the Level II Support Team and assign them to the team.
     - Confirm the assignments by clicking **Add** or **Save**.

6. **Verify Team Creation**
   - **Review Teams:**
     - Return to the **Teams** section to ensure that the **Level II Support** team appears in the list with the correct configurations.
   - **Test Ticket Routing:**
     - Submit a test ticket to verify that it is correctly routed to the **Level II Support** team based on the defined departments and permissions.

<img src="https://i.imgur.com/d7WuRn8.png" height="80%" width="80%" alt="Configuration Steps"/>

**Creating New Agents in osTicket**

To ensure efficient ticket management, it is essential to create new agent accounts within osTicket. Follow the steps below to add new agents, such as Jane Doe and John Doe, to your ticketing system.

### **Steps:**

1. **Access the Admin Panel**
   - **Log In:**
     - Open your web browser and navigate to your osTicket installation.
     - Enter your administrative credentials to log into the **Admin Panel**.

2. **Navigate to the Agents Menu**
   - **Open Agents Settings:**
     - In the Admin Panel, locate and click on the **Agents** menu. This section manages all agent-related configurations.

3. **Add New Agents**
   - **Initiate Agent Creation:**
     - Click on the **Add New Agent** button to begin creating a new agent account.
   
   - **Enter Agent Credentials:**
     - **Full Name:** Enter the agent's full name (e.g., **Jane Doe**).
     - **Email Address:** Provide a valid email address for the agent.
     - **Username:** Assign a unique username for the agent.
     - **Password:** Set a strong password for the agent account.
     - **Confirm Password:** Re-enter the password to confirm.
   
   - **Assign Roles and Permissions:**
     - Select the appropriate **role** for the agent (e.g., **Agent**, **Supervisor**).
     - Configure **permissions** based on the agent's responsibilities within the support structure.
   
   - **Save the Agent Account:**
     - After entering all necessary information, click **Save** or **Create** to finalize the agent account creation.

4. **Verify Agent Accounts**
   - **Review Agents List:**
     - Ensure that the newly created agents (**Jane Doe** and **John Doe**) appear in the **Agents** list.
   
   - **Assign to Departments or Teams:**
     - If applicable, assign the agents to specific **departments** or **teams** to streamline ticket distribution and management.


<p>
<img width="1800" alt="Screenshot 2024-12-09 at 5 02 01 PM" src="https://github.com/user-attachments/assets/59695c3d-9c38-4c7d-b66f-3f2db56d403d">
<img width="1800" alt="Screenshot 2024-12-09 at 5 09 22 PM" src="https://github.com/user-attachments/assets/60aa3b8d-da9b-4fda-b008-d043ca4dd81e">
<img width="1800" alt="Screenshot 2024-12-09 at 5 10 28 PM" src="https://github.com/user-attachments/assets/22459cd5-b4e6-4e4c-a8ff-ed550084777c">

</p>


**Creating New Users in osTicket**

In this step, we will create new user accounts in osTicket to enable users to submit tickets, which agents can then receive and triage efficiently.

### **Steps:**

1. **Access the Agents Panel**
   - **Log In:**
     - Open your web browser and navigate to your osTicket installation.
     - Enter your administrative credentials to log into the **Admin Panel**.
   
2. **Open the Users Menu**
   - **Navigate to Users:**
     - In the **Admin Panel**, locate and click on the **Agents** menu.
     - From the dropdown, select **Users** to access the user management section.
   
3. **Add New Users**
   - **Initiate User Creation:**
     - Click on the **Add User** button to begin creating a new user account.
   - **Enter User Credentials:**
     - **Full Name:** Enter the user's full name (e.g., **Karen**).
     - **Email Address:** Provide a valid email address for the user.
     - **Username:** Assign a unique username for the user.
     - **Password:** Set a strong password for the account.
     - **Confirm Password:** Re-enter the password to confirm.
   
4. **Finalize User Creation**
   - **Save the Account:**
     - After entering all necessary information, click **Save** or **Create** to finalize the user account creation.
   - **Repeat for Additional Users:**
     - Repeat the above steps to create additional users as needed (e.g., **Ken**).

<p>
<img width="1800" alt="Screenshot 2024-12-09 at 5 27 46 PM" src="https://github.com/user-attachments/assets/99287c12-7e74-4d7d-bc01-8acc13505e41">
</p>

**Creating Service Level Agreements (SLAs) in osTicket**

To effectively categorize tickets based on their level of impact, it is essential to establish Service Level Agreements (SLAs). Follow the steps below to create and configure SLAs within osTicket:

### **Steps:**

1. **Access the Admin Panel**
   - **Log In:**
     - Open your web browser and navigate to your osTicket installation.
     - Enter your administrative credentials to log into the **Admin Panel**.

2. **Navigate to the Manage Menu**
   - **Open Manage Settings:**
     - In the Admin Panel, locate and click on the **Manage** menu to access various management options.

3. **Create New SLAs**
   - **Select SLA Management:**
     - Within the Manage menu, click on **SLA** to access the SLA configuration section.
   - **Add a New SLA:**
     - Click on the **Add SLA** button to initiate the creation of a new Service Level Agreement.
   - **Define SLA Details:**
     - **Name:** Enter the name of the SLA (e.g., **SEV-A**, **SEV-B**, **SEV-C**).
     - **Response Time:** Specify the maximum time allowed to respond to a ticket (e.g., 1 hour for SEV-A).
     - **Resolution Time:** Define the target time to resolve the ticket (e.g., 1 hour for SEV-A).
     - **Priority Levels:** Assign priority levels based on the severity of the ticket.
     - **Description:** Optionally, provide a brief description of the SLA's purpose and criteria.
   - **Save the SLA:**
     - After entering all necessary details, click **Save** to finalize the SLA creation.

4. **Configure SLAs for Different Severity Levels**
   - **Create SEV-A SLA:**
     - **Name:** SEV-A
     - **Resolution Time:** 1 hour
   - **Create SEV-B SLA:**
     - **Name:** SEV-B
     - **Resolution Time:** 4 hours
   - **Create SEV-C SLA:**
     - **Name:** SEV-C
     - **Resolution Time:** 8 hours
   - **Repeat the SLA Creation Process:**
     - Follow the same steps to create each SLA, ensuring that the resolution times align with the intended severity levels.

<img width="1800" alt="Screenshot 2024-12-09 at 5 32 41 PM" src="https://github.com/user-attachments/assets/1d496c3b-273c-418e-b0c8-43ae268813ee">

**Creating Help Topics in osTicket**

Help Topics are essential for guiding users to select the appropriate category that accurately describes their issues, enabling agents to understand and address tickets efficiently. Follow the steps below to create new Help Topics within osTicket:

### **Steps:**

1. **Access the Admin Panel**
   - **Log In:**
     - Open your web browser and navigate to your osTicket installation.
     - Enter your administrative credentials to log into the **Admin Panel**.

2. **Navigate to the Manage Menu**
   - **Open Manage Settings:**
     - In the **Admin Panel**, locate and click on the **Manage** menu to access various management options.

3. **Open the Help Topics Section**
   - **Select Help Topics:**
     - Within the **Manage** menu, click on **Help Topics** to view and manage existing help topics.

4. **Create a New Help Topic**
   - **Initiate Help Topic Creation:**
     - Click on the **Add New Help Topic** button to begin creating a new Help Topic.
   
   - **Enter Help Topic Details:**
     - **Topic Name:** Enter the name of the Help Topic (e.g., **Business Critical Outage**, **Personal Computer Issues**, **Equipment Reset**, **Password Request**).
     - **Description:** Optionally, provide a brief description to help users understand when to select this topic.
     - **Category Assignment:** Assign the Help Topic to the relevant category to ensure proper ticket routing.
   
   - **Save the Help Topic:**
     - After entering all necessary information, click **Save** or **Create** to finalize the Help Topic creation.

5. **Repeat for Additional Help Topics**
   - **Add More Topics:**
     - Repeat the above steps to create additional Help Topics as needed, ensuring comprehensive coverage of common user issues.

6. **Verify Help Topics Creation**
   - **Review Help Topics List:**
     - Ensure that all newly created Help Topics appear in the **Help Topics** list with correct names and descriptions.
   - **Test Help Topic Selection:**
     - Submit a test ticket and verify that the Help Topics are available for selection, guiding users to categorize their issues accurately.

<p>
<img width="1800" alt="Screenshot 2024-12-09 at 5 46 53 PM" src="https://github.com/user-attachments/assets/4b6345a7-42c2-4f90-8d74-a0c2c056a727">
</p>

<h2>osTicket Configurations are Complete</h2>

With all configurations successfully implemented, osTicket is now fully operational as a robust ticketing system. We are equipped to create and triage tickets efficiently, simulating a real-world support environment to ensure effective issue resolution.

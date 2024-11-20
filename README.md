<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This lab demonstrates the necessary changes I make to configure osTicket so it can be used as a proper ticketing system.<br />

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
<img src="https://i.imgur.com/S33TPEZ.png" height="80%" width="80%" alt="Configuration Steps"/>
<img src="https://i.imgur.com/7HyoONM.png" height="80%" width="80%" alt="Configuration Steps"/>
</p>



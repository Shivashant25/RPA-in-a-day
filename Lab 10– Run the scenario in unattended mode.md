# Lab 10 – Run the scenario in unattended mode

# Exercise 1: Basic Desktop Flow in Unattended mode:

1. **Navigate** to https://admin.powerplatform.microsoft.com/.
1. **Click** on Resources from the menu ans 
3. If your remote VM has no Excel installed, you should disable the following steps from your desktop flow before you run them on the remote VM.
4. Start the **VM1-{Suffix}**. If it's in pause state from the **resources** tab of the environment.
   
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.11.png?raw=true)
   
1. In the search bar, **Search** for **RDP** and **select** the **Remote Connection Desktop** app.
   
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.1.png?raw=true)
   
1. From the **Environment details** tab, Copy the **VM1 DNS Name**.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.2.png?raw=true)
  
1. Paste the **VM1 DNS Name** in the **Computer** bar and **click on** on **Connect**.
   
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.3.png?raw=true)
   
1. Enter the **Username** and **Ppassword**. The Credentials are provided in the **Environment Details** tab.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.4.png?raw=true)
   
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.5.png?raw=true)
   
1. In the **Search bar**, Search for **On-premise data gateway** and **open** the app.
 
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.6.png?raw=true)
   
1. Sign into the gateway using the same account that you created in lab 1 (the one you use to sign in Power Automate portal).

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.7.png?raw=true) 
   
1. **Select** Register a new gateway on this computer, then **click Next**.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.8.png?raw=true)

1. **Name** the gateway **Test on VM gateway**. **Create** a recovery key. Then **click** Configure.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.9.png?raw=true)
   
1. **Click** Close.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.10.png?raw=true)
   
1. Now go back to the **Jump VM** computer (not VM) navigate to flow.microsoft.com. **Go to** My flows > Cloud flows.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.12.png?raw=true)

1. **Click** +New flow > Instant cloud flow.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.13.png?raw=true)
   
1. **Name** the flow as **Manual trigger Desktop flow to enter invoice on VM**, **select** Manually trigger a flow. Then **click** Create.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.14.png?raw=true)
   
1. **Click** on **+New step**.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.15.png?raw=true)
   
1. **Search** for **Desktop flows** and **select** Run a flow built with Power Automate Desktop.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.16.png?raw=true)
   
1. **Click** on the three dots and **select** Add new connection.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.17.png?raw=true)
   
1. **Select** Test on VM gateway in the Gateway name field, **enter** username (e.g. ml-refvm- 607426\rpadmin) and password. Or the VM log in credential provided by your instructor. Then **click** on Create

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.18.png?raw=true)
   
1. **Select** Enter an invoice Desktop flow.

   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.19.png?raw=true)
   
1. Fill the box with these values:
   - **Run Mode**: Unattended -Runs in the background without signing in
   - **Amount**: $200
   - **Contact**: b.friday@wingtiptoys.com b.fre
   - **Account**: WingTip Toys 

   Then **click** on save.
   
   ![](https://github.com/Shivashant25/RPA-in-a-day/blob/main/images/1.20.png?raw=true)

   

   

   
   

# Salesforce Digital Channel Configuration

## Task 01

###<code style="color : green">**Create Routing Configurations**</code>

---

* Use a browser window and [login to Salesforce](https://login.salesforce.com/) using pod credentials assigned

!!! Important
    Please contact your proctor if prompted for a Salesforce verification code.
    
* Click on the gear icon on top right corner and select Setup from the drop down menu.
* From Setup Quick Find box, search and select **Routing Configurations**
* Click on New button to create a new routing configuration.

![Nav](./assets/digTask01_1.png){ width="800" }

* Enter following details - see screenshot below 
* **Basic Information**
    - Routing Configuration Name
    - Developer Name
    - Ignore Overflow Assignee (User/Queue)
* **Routing Settings**
    - Set Routing Priority (lower number = higher priority)
    - Select Routing Model (e.g., Most Available)
    - Enter Push Time-Out (seconds) (e.g. 120 Seconds)
    - Choose Capacity Type (Inherited or Dedicated)
* **Work Item Size**
    - Enter Units of Capacity or Percentage of Capacity (only one)

* Click Save.

![Nav](./assets/digTask01_2.png){ width="1000" }


## Task 02

###<code style="color : green">**Create a Messaging Queue**</code>

---

* From Setup Quick Find box, search and select **Queues**
* Click on the New button to create a new Queue.

![Nav](./assets/digTask02_1.png){ width="800" }

* Enter following details - see screenshot below
* **Queue Name and Email Address**
    - Label (ex: SCVChatQueue)
    - Queue Name (accept auto-populated or edit)
    - Optional: Queue Email and Queue Description
* **Configuration with Omni-Channel Routing**
    - Select Routing Configuration created in the previous Step. (ex: SCVChat Routing Cfg)
* **Supported Objects**
    - Move Messaging Session from Available Objects to Selected Objects
* **Queue Members**
    - Select member type (Users / Roles / Groups)
    - Add your user(s) (ex: agents) to Selected Members

* Click Save.
![Nav](./assets/digTask02_2.png){ width="800" }


!!! Note
    You don’t necessarily need to create a new Presence Status. You can modify an existing online presence status to add Messaging Channel. If you choose this approach, you can skip next two steps and jump to task 5.   


## Task 03

###<code style="color : green">**Create a Presence Status for Messaging**</code>

---
    
* From Setup Quick Find box, search and select **Presence Statuses** and click on New button.
* Enter following details - see screenshot below
* **Basic Information**
    - Status Name (ex: Avilable Chat and Voice)
    - Developer Name (accept auto-populated or edit)
* **Status Options**
    - Select Online (to allow agents to receive work)
* **Service Channels**
    - From Available Channels, add Messaging (or both, Messaging and Phone)

* Click Save.
![Nav](./assets/digTask03_1.png){ width="800" }


## Task 04

###<code style="color : green">**Assign the Presence Status to the Agents**</code>

---
    
* From Setup Quick Find box, search and select **Permission Sets**
* Click to open Partner Telephony Permission Set
* Click Service Presence Statuses Access
* Click Edit button
* In the Available Service Presences Statuses list, select the presence status(es) previously created and click Add to associate them with the permission set. Agents who are assigned to this permission set can sign into Omni-Channel with any of the presence statuses made available to them.
* Click the Save button.

![Nav](./assets/digTask04_1.png){ width="800" }

!!! Note
    Following steps are optional if not performed in the previous lab Task 07: Assign Presence Status(es) to Agent(s)
    
* Click on Manage Assignments on the same page (screenshot above)
* Then click Add Assignment on the top right corner, select the desired user.
* Click Next, select an Expiration Option for the assigned users (Optional) and then click Assign and Done.  





## Task 0X

###<code style="color : green">**Enable Salesforce Voice - Turn on Voice with Partner Telephony**</code>

---

!!! Note
    Review (Skip if already Enabled.)

    
* From Setup Quick find box, search and select **Partner Telephony Setup** and toggle the button for Enable Service Cloud Voice.
* Scroll down to More Voice Settings section and make sure Respect Agent Capacity is Disabled or Off.

![Nav](./assets/task03_1.png){ width="800" }



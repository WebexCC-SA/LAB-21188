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

![Nav](./assets/digTask01_2.png){ width="800" }


## Task 02

###<code style="color : green">**Enable Omni-Channel**</code>

---

!!! Note
    Review (Skip if Omni-Channel setting is already Enabled.)


* From Setup Quick Find box, search and select **Omni-Channel Settings**
* Move the slider to enable Enhanced Omni-Channel Routing.
* Select Enable Omni-Channel and Click Save.

![Nav](./assets/task02_1.png){ width="800" }


## Task 03

###<code style="color : green">**Enable Salesforce Voice - Turn on Voice with Partner Telephony**</code>

---

!!! Note
    Review (Skip if already Enabled.)

    
* From Setup Quick find box, search and select **Partner Telephony Setup** and toggle the button for Enable Service Cloud Voice.
* Scroll down to More Voice Settings section and make sure Respect Agent Capacity is Disabled or Off.

![Nav](./assets/task03_1.png){ width="800" }



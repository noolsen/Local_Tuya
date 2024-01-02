# Local Tuya Installation

[Other guide in english, used as inspiration:](https://smarthomecircle.com/how-to-setup-local-tuya-in-home-assistant)

[If you are using a FESH item:](https://fesh.dk/hjaelpecenter/hvordan-flytter-jeg-min-produkter-til-et-andet-wi-fi-netvaerk/)
The following is shown for a FESH light bulb.

## Move the bulb to your own network

Download the app: **Smart Life**
and connect your bulb in the app - shows the FESH bulb

## Install LocalTuya in Home Assistant

In *Home Assistant*, *HACS* install: **LocalTuya**

- Click on![Tryk på](Images/HACS_LocalT_Inst.png)

- Find:  ![Alt text](Images/LocalTuya_App.png)

- Restart *HA*

- In *Settings*, *Installation* click on: ![Alt text](<Images/Add Integration.png>)

- Look for LocalTuya:

    ![](<Images/Search LocalTuya.png>)

## Settings for LocalTuya

- Start configuration of Local Tuya – remember to mark ”Do not configure …”
![Alt text](Images/ConfigureTuya.png)

  and click on: *Submit*

    ![Alt text](Images/ConfigureTuya_Succes.png)
  
  Click on: *Finish*

- Open Local Tuya ![Alt text](Images/Abn_LocalTuya.png)

- Click on *Configure* and mark: Add new Device

    ![Alt text](Images/AddNewDevice.png)
  
  Click on: *Submit*
  Local Tuya will now find the new device with its IP-adress. Click on: *Submit*
  
- Insert a name for the device
    
    ![Alt text](Images/ConfigureTuyaDevice1.png)
  
  Now we have to find the Local Key.

- Create a Tuya account at:  https://iot.tuya.com/

- After creation of your account click on: *Cloud*, *Development*

    ![Alt text](Images/TuyaDevelopment.png)

- Create a Cloud Project, click on:  ![Alt text](Images/CreateCloud.png)

- Fill in the the formular, remember *Data Center* and click on: Create

    ![Alt text](Images/CreateCloudProject.png)

- Now a window: *Authorize API services* appears, click on: *Authorize*
- In the windowwith your new project, click on the tab: *Devices*

    ![Alt text](Images/Devices1.png)

    ![Alt text](Images/Devices_2.png)

- Click on the tab: *Link Tuya Account* and the button: ![Alt text](Images/AddAppAccountBut.png)

  The following window is shown:

  ![Alt text](Images/ScanCode1.png)

- Now open the *Smart Life* app. At *Home* choose "+" and *Scan*.
  
  Scan the QR coode.

- At the *Tuya* platform the following window is shown:

  ![Alt text](Images/LinkTuyaAccount.png)
  
  Click on: *OK*

  ![Alt text](Images/ManageDevice1.png)
  
  Click on: "X"

- Now your device is shown:

  ![Alt text](Images/LocalTuyaDeviceShow1.png)

  Your app is now linked to the cloud project.

- Click on the tab: *All Devices* and the device is shown.

  ![Alt text](Images/AllDevices1.png)

  Copi the *Device ID*.

- Click on:

  ![Alt text](Images/CloudAPIExplorer.png)

- In the new window choose:

  ![Alt text](Images/DeviceID1.png)
  
  and insert the devide-id.

  Click on: ![Alt text](Images/SubmitRequest.png)

- In the next window you can see the *Local Key* for the device:

  ![Alt text](Images/LocalKey1.png)

  Copy the local_key.

- Back in HA insert the *Local Key*

  ![Alt text](Images/DeviceLocalKey1.png)

  Click on: *Submit*

- Choose an *Entity Type*

  ![Alt text](Images/EntityType.png)

  Click on *Submit*

- The enntity has now to be configured depending on the device type. At [GitHub](https://www.markdownguide.org/cheat-sheet/) you can find proprosals for different devices.

  Here the values for a ligt-bulb are used:

  ![Alt text](Images/ConfigureEntity.png)

  You do not need to fill out *Scene*, click on *Submit*. Enter entity-type again, click *Submit*. Now you get:

  ![Alt text](Images/Succes.png)

  Click on: *Finish*

- At *Setting*, *Devices* the configured device is now shown.

  ![Alt text](Images/SettingDevices.png)

  Open the device and *Device Info* is shown:

  ![Alt text](Images/DeviceInfo.png)

  Click on the light-bulb and it can now be set up:

  ![Alt text](Images/FESHFinish.png)

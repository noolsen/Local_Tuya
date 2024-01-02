# Local Tuya Installation

[Guide på engelsk:](https://smarthomecircle.com/how-to-setup-local-tuya-in-home-assistant)

[Hvis du har en FESH enhed:](https://fesh.dk/hjaelpecenter/hvordan-flytter-jeg-min-produkter-til-et-andet-wi-fi-netvaerk/)
Jeg har en FESH pære

## Flyt pæren over til eget netværk

Download appen: **Smart Life**
og connect pæren i appen - finder FESH pæren

## Installere LocalTuya i Home Assistant

I Home Assistant i HACS installeres: **LocalTuya**

- Tryk på![Tryk på](Images/HACS_LocalT_Inst.png)

- Find:  ![Alt text](Images/LocalTuya_App.png)

- Genstart HA

- I Settings, Installation tryk på: ![Alt text](<Images/Add Integration.png>)

- Søg efter LocalTuya:

    ![](<Images/Search LocalTuya.png>)

## Opsætning af LocalTuya

- Start configuration af Local Tuya – husk at markere ”Do not configure …”
![Alt text](Images/ConfigureTuya.png)

  og tryk på: Submit

    ![Alt text](Images/ConfigureTuya_Succes.png)
  
  Tryg på: Finish

- Åbn Local Tuya ![Alt text](Images/Abn_LocalTuya.png)

- Tryk på Configure og marker: Add new Device

    ![Alt text](Images/AddNewDevice.png)
  
  Tryk på: Submit
- Local Tuya finder den nye device med IP-adresse. Tryk på: Submit
  I skærmbilledet indtastes et navn for Device
    
    ![Alt text](Images/ConfigureTuyaDevice1.png)
  
  Nu skal  Local Key findes.

- Opret en Tuya account på:  https://iot.tuya.com/

- Efter oprettelse af account tryk på: Cloud, Development

    ![Alt text](Images/TuyaDevelopment.png)

- Opret et Cloud Project, tryk på  ![Alt text](Images/CreateCloud.png)

- Udfyld formular, husk Data Center og tryk på: Create

    ![Alt text](Images/CreateCloudProject.png)
- Der dukker nu et billede op med: Authorize API services, tryk på: Authorize
- I billedet med det oprettede projekt tryk på Devices:

    ![Alt text](Images/Devices1.png)

    ![Alt text](Images/Devices_2.png)

- Tryk nu på Link Tuya Account og knappen: ![Alt text](Images/AddAppAccountBut.png)

  Følgende billede vises:

  ![Alt text](Images/ScanCode1.png)

- Åbn nu *Smart Life* appen. Under *Home* vælg "+" tegnet og *Scan*
  Scan QR koden

- I *Tuya* platformen vise nu billedet:

  ![Alt text](Images/LinkTuyaAccount.png)
  Tryk på *OK*

  ![Alt text](Images/ManageDevice1.png)
  Tryk på "X"

- Nu vises devicen i flg. billede:

  ![Alt text](Images/LocalTuyaDeviceShow1.png)

  Appen er nu linket til cloud projektet.

- Klik på fanen *All Devices* og du kan se din device

  ![Alt text](Images/AllDevices1.png)
  Marker *Device ID* og kopier id'en.

- Klik nu på:

  ![Alt text](Images/CloudAPIExplorer.png)

- I det nye billede vælges:

  ![Alt text](Images/DeviceID1.png)
  
  og den kopierede ID indsættes.

  Tryk på: ![Alt text](Images/SubmitRequest.png)

- I flg. billede set devicens UUID:

  ![Alt text](Images/UUID1.png)

  Kopier UUID'en.





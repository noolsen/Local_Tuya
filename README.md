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
- Tryk på Configure og marker: Add new Device![Alt text](Images/AddNewDevice.png)
  
  Tryk på: Submit
- Local Tuya finder den nye device med IP-adresse. Tryk på: Submit
  I skærmbilledet indtastes et navn for Device
    
    ![Alt text](Images/ConfigureTuyaDevice.png)
  
  Nu skal  Local Key findes.

- Opret en Tuya account på:  https://iot.tuya.com/

- Efter oprettelse af account tryk på: Cloud, Development

    ![Alt text](Images/TuyaDevelopment.png)

- Opret et Cloud Project, tryk på  ![Alt text](Images/CreateCloud.png)

- Udfyld formular, husk Data Center og tryk på: Create

    ![Alt text](Images/CreateCloudProject.png)
- Der dukker nu et billede op med: Authorize API services, tryk på: Authorize
- I billedet med det oprettede projekt tryk på Devices:

    ![Alt text](Images/Devices.png)



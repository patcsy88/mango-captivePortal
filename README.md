# mango-captivePortal

Set up of Mango with OpenWRT to 'proxy' campus Captive Portal

1. Connect to the secured WiFi SSID 9dot1. Please contact me for the password.

2. Using your favourite browser, go to http://192.168.9.1 (it should get re-directed to https://192.168.9.1. Since it is aself-signed cert, you can accept the browser warning and proceed.

3. The following login screen should appear 
<img width="1375" alt="Screenshot 2023-01-30 at 2 02 13 PM" src="https://user-images.githubusercontent.com/30426256/215399209-90891fbf-33af-4434-a84f-84482822a751.png">

4. At this point it has not been secured with a password, so go ahead and click Login to log in.

5. You should now be at the Status => Overview page
<img width="958" alt="Screenshot 2023-01-30 at 2 08 33 PM" src="https://user-images.githubusercontent.com/30426256/215400515-b9b2e324-ab9b-41bb-b0f9-5831cb9f69cb.png">

6. Navigate to Services => Travelmate
<img width="983" alt="Screenshot 2023-01-30 at 2 09 41 PM" src="https://user-images.githubusercontent.com/30426256/215400787-55e08807-ebdf-45fe-aa3a-8e98d90d48ba.png">

7. Change to the Wireless Stations tab and click Scan on radio0
<img width="947" alt="Screenshot 2023-01-30 at 2 09 56 PM" src="https://user-images.githubusercontent.com/30426256/215400793-cdd1bee8-4a3d-4680-a4b6-380803742f39.png">

8. Select the WiFi SSID you want to connect to and click "Add uplink..."
<img width="1638" alt="Screenshot 2023-01-30 at 2 10 07 PM" src="https://user-images.githubusercontent.com/30426256/215400817-933b582a-6467-4a0c-96eb-7f348c9f3c76.png">

9. Leave the pre-polulated information unchanged. Click Save.
<img width="1623" alt="Screenshot 2023-01-30 at 2 10 15 PM" src="https://user-images.githubusercontent.com/30426256/215400830-d05b6ee3-9a2d-4a1e-a214-5658205ba298.png">

10. Check that the uplink information appears correct and then click "Save & Apply"
<img width="957" alt="Screenshot 2023-01-30 at 2 10 26 PM" src="https://user-images.githubusercontent.com/30426256/215400844-435bf250-9155-4766-8298-53e82e52ae19.png">

11. Selecting the Overview tab, you should see the Status/ Version as Connected.
<img width="970" alt="Screenshot 2023-01-30 at 2 20 31 PM" src="https://user-images.githubusercontent.com/30426256/215403022-35a6e49f-a720-45d5-9b85-f588c3612715.png">

12. If all goes well, the Captive Portal should now popup.
<img width="900" alt="Screenshot 2023-01-30 at 2 20 07 PM" src="https://user-images.githubusercontent.com/30426256/215403148-9907dd59-6d69-4239-a804-199b0812a75b.png">

13. If for whatever reason the Captive Portal popup doe not appear on your Mac/Computer, using your favourite smartphone, connect the same WiFi SSID with the appropriate password. The Captive Portal popup should appear once the WiFi is connected.

14. Enter the appropriate credentials or voucher, and if the Captive Portal authentication/authorization is successful, the Mango is now ready to 'proxy' all client (stations) connected to the Mango's WiFi "9dot1".

Should the above not work, the following are several troubleshooting steps

1. DNSMasq Setup
Ignore resolv file should NOT be selected and the Resolv file path should be empty
<img width="970" alt="Screenshot 2023-01-30 at 2 28 42 PM" src="https://user-images.githubusercontent.com/30426256/215404406-5906952c-3472-4dd8-8caa-32fe479051e6.png">

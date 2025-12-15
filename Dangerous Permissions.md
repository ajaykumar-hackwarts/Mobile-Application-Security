In Android, permission is what the app is allowed to do and what it can access. And these dangerous permissions are listed in the androidmanifest.xml.

1. ACCESS_FINE_LOCATION : Use to access user's precise physical location.
   
<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Maps and navigation</td>
    <td>Google map, Rapido, Zomato</td>
    <td>Surveilence, stalking and profiling</td>
  </tr>
</table>


2. ACCESS_COARSE_LOCATION : Use to access user's approxiamte physical location.  

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Weather forecast, regional specific news</td>
    <td>Weather apps, news apps</td>
    <td>Profiling, behavioral tracking not much threat</td>
  </tr>
</table>



3. ACCESS_BACKGROUND_LOCATION : Use to access user's location even the app is not visible or in use.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Fitness & Health tracking, vehicle tracking</td>
    <td>Strava, Find My Device</td>
    <td>Continous surveillance or spying</td>
  </tr>
</table>


4. RECORD_AUDIO : Use to access the device microphone and record the audio.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Video calls, Voice assistant etc...</td>
    <td>Whatsapp, Google assistant etc...</td>
    <td>spying, data exfiltration/threat</td>
  </tr>
</table>


5. CAMERA : Use to access the device camera to capture photos and videos. 

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Camera & Video call apps, Barcode & Document scanning</td>
    <td>Camera app, Instagram, snapchats etc...</td>
    <td>Recording video and taking photo secretly and doing Spyware</td>
  </tr>
</table>

6. READ_PHONE_STATE : Use to access telephony information about the device like wheather a call is active, idle or ringing, outgoing or incoming, IMEI(International Mobile Equipment Identity), IMSI(International Mobile Subscriber Identity), Phone number, SIM information.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Pause music or video when incoming or outgoing calls, monitor network and sim status</td>
    <td>Spotify, Youtube or any media player apps, Whatsapp, Banking apps for device authentication</td>
    <td>Monitoring call activity, Track users accross apps by collecting IMEI so even when the app is uninstalled we can identify the device.</td>
  </tr>
</table>
  
7. CALL_PHONE : Use to directly make a phone call without the user interaction using the device's dialer.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Emergency calls, vehicle hand-free calls</td>
    <td>SOS apps, Saftey apps</td></td>
    <td>Premium call fraud, call state monitoring, costs money.</td>
  </tr>
</table>


8. READ_CALL_LOG : Use to read the device's call history including incoming, outgoing and missed calls.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Default dialer apps, call history and backup apps.</td>
    <td>Google Phone, True caller</td> 
    <td>Spying on who you communicate with, Tracking call frequency and habits.</td>
  </tr>
</table>


9. WRITE_CALL_LOG : Use to modify the device's call history like add, edit and delete call logs.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Restore call history after reset, transfer call logs to new device</td>
    <td>Google Phone, Nothing Phone</td> 
    <td>Hiding premium calls, Inserting fake call evidence.</td>
  </tr>
</table>

10. ANSWER_PHONE_CALLS : Use to programmatically answer incoming calls without the user touching the screen.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Accessibility, Emergency, Driving, VOIP apps.</td>
    <td>Google Assistant, Android Auto, SOS apps.</td> 
    <td>Spyware auto-answer calls to listen without users knowledge, Record the calls with secretly when combined with record_audio</td>
  </tr>
</table>


11. READ_SMS : Use to read all the stored messages in the device.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging, Banking, two factor authentication apps.</td>
    <td>Whatsapp, Truecaller</td> 
    <td>Steals OTP, personal, financial messages and forward to 3rd party server without users concern.</td>
  </tr>
</table>
 
12. RECEIVE_SMS : Use to access all the incoming messages in the device.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging, Banking, Delivery and two factor authentication apps.</td>
    <td>Whatsapp, Google Authenticator, True Caller</td> 
    <td>Collects the OTP and to bypass 2FA, Read confidential messages.</td>
  </tr>
</table>

13. SEND_SMS : Use to send the messages from the device without user's intervention.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging, Banking, Delivery and two factor authentication apps.</td>
    <td>Whatsapp, Banking apps, Mobile device management apps.</td> 
    <td>Spyware like exfiltration of messages like OTP, financial and personal messages.</td>
  </tr>
</table>

14. RECEIVE_MMS : Use to access the incoming MMS(multimedia messaging services) messages like images, video, audio, text etc...

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Default messaging apps, Enterprise messaging apps</td>
    <td>Whatsapp, Google chat, Microsoft Teams.</td> 
    <td>Spy on user by reading attachement, Upload them to remote server</td>
  </tr>
</table>



15. READ_CONTACTS : Use to read the user's contacts stored on the device.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging, email and social media apps</td>
    <td>Whatsapp, Facebook, Gmail </td> 
    <td>Harvesting contacts for phishing attacks, Selling contacts to third party attacks</td>
  </tr>
</table>


16. WRITE_CONTACTS : Use to add, edit or delete contacts on the device. 

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging apps to add new contacts from invite links, sync contacts in social media.</td>
    <td>Whatsapp, Facebook.</td> 
    <td>Spam contact injection, phishing, exfiltration</td>
  </tr>
</table>


17. READ_EXTERNAL_STORAGE : Use to read files on the external storage like SD card or device storage.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Media player, Gallery, Photo editing</td>
    <td>VLC, MX player, PicsArt</td> 
    <td>Viewing personal photos, Reading sentive documents</td>
  </tr>
</table>


18. WRITE_EXTERNAL_STORAGE : Use to add, delete or edit files on the external storage like sd card or device storage.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>File manager, document apps.</td>
    <td>Gallery to save edited images, MX player</td> 
    <td>Deleting user files, encrypt user files and demand payment.</td>
  </tr>
</table>


19. READ_MEDIA_IMAGES/READ_MEDIA_VIDEO/READ_MEDIA_AUDIO : Use to read image, video and audio files already stored on the device.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Media & Music player, Gallery, Photo editing, Social media</td>
    <td>MX player, Spotify, Whatsapp, Gallery, Camscanner</td> 
    <td>Analyse image for credentials, Sensitive photo, video and audio exfiltration.</td>
  </tr>
</table>


20. READ_CALENDAR : Use to read the user's calender events and details like titles, times and locations.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Calender, email and meeting apps</td>
    <td>Google Calender, Microsoft teams, Gmail</td> 
    <td>Viewing personal shedules, profiling, social engineering, phishing.</td>
  </tr>
</table>

 
21. WRITE_CALENDAR : Use to modify the user's calender and details like titles, times and locations.


<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Calender, email and meeting apps</td>
    <td>Google Calender, Microsoft teams, Gmail</td> 
    <td>Deleting or modifying important events, phishing.</td>
  </tr>
</table>


22. SYSTEM_ALERT_WINDOW : Use to display content over other apps like floating windows, chat heads or bubbles, persistant overlays etc.


<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Chat bubbles, floating utilities like volume, calculator</td>
    <td>Facebook, Floating calculator, notes</td> 
    <td>Clickjacking, Phishing, Making an overlay like click okay to fix and it can lock the device then asking for ransom.</td>
  </tr>
</table>


23. BIND_ACCESSIBILITY_SERVICE : Use to observe what is on your device screen and interact with the apps on your behalf.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Assist users with disabilities</td>
    <td>Talk back, voice access, maginfier</td> 
    <td>Full device take over, Credentials theft, Phishing, ransomware</td>
  </tr>
</table>

24. BIND_DEVICE_ADMIN : Use to became a device administrator like having all the privileges on the device. 

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Corporate device management.</td>
    <td>Microsoft Intune</td> 
    <td>Data theft, Device lockout, Ransomware.</td>
  </tr>
</table>
 
25. REQUEST_IGNORE_BATTERY_OPTIMIZATIONS : Use to ask the system to exclude it from the battery-saving restrictions.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Messaging, Navigation and Device management apps.</td>
    <td>Whatsapp, Map, Screen Recorder.</td> 
    <td>Stealth spyware, Persistant malware and battery drain.</td>
  </tr>
</table>

 
26. BIND_TELECOM_SERVICE : Use to connect to phone'e telecom services like managing phone calls, accessing call-related info, VOIP calls.

<table>
  <tr>
    <td>Legitimate Purpose</td>
    <td>Examples</td>
    <td>Threats</td>
  </tr>
  <tr>
    <td>Default Dialer apps, Call Recording apps</td>
    <td>Google Phone, Skype, Google Voice</td> 
    <td>Call interception, spoofing, privacy invasion.</td>
  </tr>
</table>


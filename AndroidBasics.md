Android is mobile operating system developed by google based on Linux kernel. Open-source and widely used in smartphones, tablets, TVs, and wearable devices.

# Core Components : 

<table>
  <tr>
    <td><strong>1. Activities</strong></td>
    <td>Represents a single screen in the UI example : login screen, setting screen etc.</td>
  </tr>
  <tr>
    <td><strong>2. Services</strong></td>
    <td>Run in the background without UI example : music playing in background when we using another application.</td>
  </tr>
  <tr>
    <td><strong>3. Broad Receivers</strong></td>
    <td>It's a notification system it triggers when an event is happened. example : alerts your phone when battery is down, receives a text message triggers a notification.</td>
  </tr>
  <tr>
    <td><strong>4. Content Providers</strong></td>
    <td>It's a data source or library or a data store that multiple people can access. example : Contacts app provides your contact list to WhatsApp or Gmail.</td>
  </tr>
</table>


# Additional Components : 

## 5. Intent : 

- Intents : It is a communication mechanism (bridge) that carries information from one component to another. 

- Types of Intents : 

1. Explicit Intent : You specify the exact component to start and this is used to send information from one activity to another in same application. 

Example : In Flipkart from choosing "view cart" button it is going to cart activity.


2. Implicit Intent : You did not specify the exact component instead you declare a general action and android finds a suitable component (might be within the app or another app.) to perform it.

Example : You click a share button on photo and android shows a list of apps(whatsapp, gmail) to share the photo.

- Intent Filter : It's a declaration in AndroidManifest.xml which tells the android which type of intents a component(activity, service, broadcast receiver) can handle. 

Example : With the same above example the list of app's manifest will have the intent filter will say that I can handle this like share the photo.


3. Pending Intent : It's a wrapper around a regular intent that allows another app or the system to execute the intent later

Example : Setting an alarm and closing the clock app and it will trigger at the time. Notification came and later when we click only it will go to the chat activity in an application.


## 6. Fragments : 

Reusable portion of an Activity's UI a part of Activity which has its own layout, lifecycle and logic inside the activity. 

Example : In WhatsApp Chat, Status and Call fragments are there inside the mainactivity. 


## 7. View & View Group : 

View is the basic building block of UI. It represents the single visual element on the screen like button, toggle switch, text, image etc.


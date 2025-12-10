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


# Additional Components: 

## 5. Intent : 

- Intent : It is a communication mechanism (bridge) that carries information from one component to another. 

- Types of Intent : 

1. Explicit Intent : You specify the exact component to start and this is used to send information from one activity to another in same application. 

Example : In Flipkart from choosing "view cart" button it is going to cart activity.


2. 
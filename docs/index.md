![](.\img\xdrip4ios.jpg)

# Introduction

**xDrip4iOS** (also known as **"xDrip for iOS"** or **"xdripswift"**) is an open-source application to display real time blood glucose data.

<img src=".\img\xDrip4iOS_env.png" style="zoom:67%;" />

It is able to connect as a **Master** device to various types of Continuous Glucose Monitor systems and display their values on the screen. This is the main way that most people (usually patients with Type 1 Diabetes) will use the app.

It is also able to act as a **Follower** device and pull remote CGM data from [Nightscout](https://nightscout.github.io/). This is a great way for parents and care-givers to be able to remotely monitor loved ones and patients.

!!!info "FOR XDRIP+ USERS"
    Please note that **xDrip4iOS** is not related to the **xDrip+** project for **Android**.

    For help and information about the **xDrip+** project for Android, please see [here](https://github.com/NightscoutFoundation/xDrip) or look on [Facebook](https://www.facebook.com/groups/xDripG5).

___
## What Do I Need?

To run xDrip4iOS you will firstly need an iPhone 7 or newer running minimum iOS13.

To work as a **Master** device, you will need to have a compatible CGM system (see below). If you want to share your CGM data with Nightscout, then you will also need a working internet connection.

To work as a **Follower** device, you don't need anything except an internet connection and a working Nightscout site from where to follow the master device.

That's it. Nothing else is needed.

!!!warning "IMPORTANT"
    **Before using xDrip4iOS**, it is important to understand several points:

    - This is an open-source, community-based project and is not supported by any company
    - It is not officially approved or regulated for diabetes therapy and/or treatment in any way whatsoever
    
    **You must understand that you take full responsibility for using this software and you agree to do so at your own risk.**

___
## Compatible Sensors

xDrip4iOS is compatible with many Libre sensors and also certain Dexcom sensors/transmitters.

### Libre 
**Libre 1 *(European 14 day)***

| Transmitter Type &nbsp;&nbsp;&nbsp;| Firmware Version &nbsp;&nbsp;&nbsp;| Compatible? &nbsp;&nbsp;&nbsp; |
|:-------------- |:------------- | :----------- |
| MiaoMiao 1, 2, 3  | All | **<span style="color:green">Yes</span>** |
| Bubble, Bubble mini | All | **<span style="color:green">Yes</span>** |
| Atom | All | **<span style="color:green">Yes</span>** |
| GNSentry | All | **<span style="color:green">Yes</span>** |

</br>

**Libre 1 *(US 14 days)* and 2 *(European 14 day)***

| Transmitter Type &nbsp;&nbsp;&nbsp; | Firmware Version &nbsp;&nbsp;&nbsp; | Compatible? &nbsp;&nbsp;&nbsp; |
| :------------------------------------ | :---------------------------------- | :----------------------------- |
| Direct Bluetooth (no transmitter)&nbsp;&nbsp;&nbsp; | -                                 | **<span style="color:green">Yes</span>** *(2)* |
| MiaoMiao 1                                          | >= 39                           | **<span style="color:green">Yes</span>** *(1)*             |
| MiaoMiao 2                                          | >= 7                             | **<span style="color:green">Yes</span>** *(1)*          |
| Miaomiao 3 | - | **<span style="color:green">Yes</span>** *(1)* |
| Bubble, Bubble mini                               | All                              | **<span style="color:green">Yes</span>**                        |
| Atom                                                | All                              | **<span style="color:green">Yes</span>**                        |
| GNSentry                                            | -                                | **<span style="color:red">No</span>**                             |

</br> 
 *(1)* The MiaoMiao firmware can be upgraded, if needed, using Tomato App

 *(2)* Only Libre 2 Europe</br>
</br>

**Libre 2 US/CA/AUS, Libre Pro, Libre H**

- **<span style="color:red">Not compatible</span>**
</br> </br> 

### Dexcom 
**Dexcom G4** *(1)* **/ G5**

- **<span style="color:green">Fully compatible</span>** with a bridge/Wixel device and using raw data mode.</br> 

**Dexcom G5**

- **<span style="color:green">Fully compatible</span>** using raw mode.
  

**Dexcom G6  and ONE**

- **<span style="color:green">Fully compatible</span>** using either raw data or native modes (see below).

Older 80xxxx/81xxxx G6 transmitters can work in **raw mode** with the possibility of processing all data using the xDrip algorithm and manual calibration. Sensor session limits do not apply in this mode.

Newer G6 "Firefly" transmitters (>8Gxxxx) and ONE will only work in **native mode** using the algorithm inside the transmitter. This means that xDrip4iOS will be limited to the factory 10 day sensor sessions and is also able to start/stop sensor sessions as well as calibrating.

If you need to use the official Dexcom app to upload data to Dexcom Share or Clarity, you can set xDrip4iOS to "Follow Dexcom App" mode. In this mode, the main connection between the transmitter and your iPhone is handled by the Dexcom app. xDrip4iOS will simply receive a copy of the transmitted data. This allows you to use xDrip4iOS for all features (alarms, graphs, statistics, Nightscout, Watch app etc) without needing to stop using the official app.
</br>

___
## Where Can I Get Help?

The main public support group for all support is the xDrip4iOS group on [Facebook](https://www.facebook.com/groups/853994615056838). Feel free to join the group, ask questions and participate.

You can also find all source code, technical information and register issues in our  [Github repository](https://github.com/JohanDegraeve/xdripswift).
</br>

___
## Development History

This project was started back in 2017 by **Johan Degraeve**. His idea was to port the original [xDrip](http://stephenblackwasalreadytaken.github.io/xDrip/) algorithm to iOS.

The original project he created was called **[xdripiosreader](https://github.com/JohanDegraeve/iosxdripreader)**. This was later re-written in 2019 into native swift code and renamed to **xdripswift**.

In 2020, the user interface was overhauled, more features were added and the user-facing project was renamed to **xDrip4iOS**.

___
## How Can I Get Involved?

You'll find the Github source repository for this documentation [here](https://github.com/paulplant/xdrip4ios_docs). Please don't hesitate to improve or correct anything you see and create a pull request!

You're also welcome to contribute or report any documentation error, unclear explanation, typo, broken link etc by going to Github and opening an [issue](https://github.com/paulplant/xdrip4ios_docs/issues).
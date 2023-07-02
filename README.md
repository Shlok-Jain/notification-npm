
# NotificationJS

This is a javascript library for showing notifications in javascript apps, React apps and many more..... It has many features like swipe for touch devices, light and dark themes, four templates for different notifications( normal, alert, error, success), compatible on all major devices. I hope you will like it.




## Authors

- [@Shlok_Jain](https://www.github.com/Shlok-Jain)


## Demo

Playground - https://shlok-jain.github.io/Notification-library#demo

![demo](https://i.postimg.cc/vHHRDJnw/Screenshot-2023-03-25-122826.png)


## Features

- Swipe to close on touch devices
- You can choose from two themes(light,dark)
- Pause timer when window loses focus
- Close Button for closing notification
- Different types of notifications for different type of messages( normal, alert, error, success )
- You can manually close notification( .hide() method)hover on notification to pause timer
- You can specify time to show notification
- and many more.....

## Installation

Install NotificationJS with npm

```bash
npm i notification-npm
```

Install NotificationJS with cdn

```html
<script src="https://cdn.jsdelivr.net/gh/Shlok-Jain/Notification-library@latest/index.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/Shlok-Jain/Notification-library@latest/index.css">
```
    
## Usage

Basic Usage
```javascript
import React from 'react'
import NotificationJS from 'notification-npm'
import '/node_modules/notification-npm/index.css'

export const Component = () => {
    const shownotification = ()=>{
        const notification = new NotificationJS({
            message: 'This is a normal notificaion',  //specify message here
            type: 'normal',                          //specify type of notification
            duration: 5000,                          //duration in milliseconds
            theme: 'dark',                           //theme of notification
            sound: true,                             //for notificaion sound
            disable_timer:false,                     //set it true of you don't want timer
        })

        notification.show()
  }

  return(<button onClick={()=>shownotification()}></button>)
}
```
[Click here to see more](https://shlok-jain.github.io/Notification-library/#usage)


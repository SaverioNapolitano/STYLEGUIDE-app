# STYLEGUIDE-app 

Files for downloading or customizing the mobile app of the [STYLEGUIDE](https://github.com/SaverioNapolitano/STYLEGUIDE.git) project. 

> [!IMPORTANT]
> Currently the app works only for Android devices. 

> [!CAUTION]
> Prior to using the app you have to change the MQTT broker and REST server addresses in the settings screen of the app (basic changes) or by modifying the `.aia` file (deeper changes). 

## Purpose 

The app allows the user to check their consumption (as long as their bill) and to manage the status, color and intensity of their lights. 

It also allows them to see what colors they use the most along with their most used methods to turn the lights on. 

## How it works 

Information about current light status, color and intensity (both incoming and outgoing) and number of people in the room (only incoming) are handled using MQTT protocol. 

All the other information are only incoming and use HTTP protocol to send requests to the [server](https://github.com/SaverioNapolitano/STYLEGUIDE-server.git)

Apart from some UI changes, the retrieved information are explained [here (HTTP)](https://github.com/SaverioNapolitano/STYLEGUIDE-server?tab=readme-ov-file#http-client) and [here (MQTT)](https://github.com/SaverioNapolitano/STYLEGUIDE-bridge?tab=readme-ov-file#mqtt)

Besides, through the app the user can specify whether they want to enable or disable the auto mode.

> [!NOTE]
> Due to this app being just a prototype and considered the obstacles faced during its development, it doesn't allow the user to see neither the energy savers ranking nor the energy saving tips. Please refer to the server repo for those.

## Further improvements 

- [ ] Code the application using a proper (multiplatform) programming language (Flutter)
- [ ] Redesign the UI 
- [ ] Allow the application to display ranking and energy saving tips
- [ ] Allow the user to specify preferences and custom routines
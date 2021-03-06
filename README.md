# ContactApp
ContactApp uses Bluetooth proximity measurements, in order to track social distancing and help people identify which activities pose the most risk.

## Download
Right now the best way to download ContactApp is directly from GitHub [here](https://github.com/nathanww/ContactApp/blob/master/app-release.apk?raw=true) since Google Play is barring COVID-related apps. To install ContactApp, you will probably need to enable apps from [unknown sources](https://www.technipages.com/where-did-allow-installation-from-unknown-sources-go-in-android).

![Screenshot](screenshot2.png?raw=true)
## Inspiration

A challenge in implementing social distancing is that it is difficult to understand how epidemiological goals (“reduce contact by 75%”) translate into recommendations (“Is it OK to go for a walk? Should I take the train?”).   This uncertainty can lead to noncompliance, for instance if people believe that going to a park does not pose a risk.

ContactApp aims to clarify social distancing and incentivize people to reduce their risk the same way fitness trackers incentivize exercise--by quantifying and tracking potentially risky close contacts and computing an “exposure score”. 

## What it does
When running in the background on an Android phone, ContactApp performs Bluetooth scans to identify nearby personal devices (wearables, phones, fitness trackers, headphones, etc). ContactApp uses signal strength to identify devices at “close contact” range, and converts the number and duration of contacts into an “exposure score” which is updated throughout the day.

Notably, this approach is anonymous by design, and does not rely on sharing GPS data, which may raise privacy concerns.

## What's next for ContactApp
I am working on a data logging mode to assist public health departments. In this mode, a low-cost Android device is placed in a public area (i.e. an office) and logs the number of devices it sees. This can be used to assess the effectiveness of policies--i.e. How much does a stay at home order reduce traffic to a location?

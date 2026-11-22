# G-Motion Privacy Policy

**Last updated:** November 22, 2026
**Developer:** iiRG4 (https://github.com/iiRG4)
**Applies to:** G-Motion v1.4.0 for Windows

This policy explains what information G-Motion uses, where it goes, and what stays on your computer.

## Summary

- G-Motion does not require an account, and it does not show ads.
- Your videos, wallpapers, and settings stay on your computer.
- The only personal data G-Motion can send over the internet is your **approximate location**, and only for the weather features.

## 1. Data that stays on your device

G-Motion stores the following in its data folder on your computer (for the Microsoft Store version, Windows keeps this folder inside the app's own package data):

- your settings and widget choices;
- your wallpaper library (paths and links to videos you add);
- thumbnails created from your videos;
- videos you send from your phone using the optional Phone Remote.

This data is not uploaded to the developer or to any other server. When you uninstall the Microsoft Store version, Windows removes this data together with the app. (If you use a version installed outside the Store, delete the `%APPDATA%\G-Motion` folder to remove it.)

## 2. Weather features (approximate location)

If you use the Weather widget or the weather-based effects, G-Motion sends a request to the G-Motion weather service (hosted on Cloudflare Workers). The request contains:

- the G-Motion version number;
- your **approximate location**: coordinates rounded to two decimal places, read from the Windows Location service (G-Motion runs Windows PowerShell to read it).

If Windows Location is turned off or unavailable, no coordinates are sent. In that case the service may estimate your location from your IP address.

Like any internet request, your IP address is visible to the services that receive it. The G-Motion weather service uses it to limit the number of requests. G-Motion has no accounts, so this information is not linked to your name or identity.

To answer the request, the weather service contacts:

- **WeatherAPI.com**, to get the weather for the approximate location (https://www.weatherapi.com/terms.aspx);
- **OpenStreetMap Nominatim**, to turn the coordinates into a city name (https://operations.osmfoundation.org/policies/nominatim/).

You can stop all of this by turning off the Weather widget and the weather effects, or by turning off Windows Location.

## 3. Video links you add

If you add a video from a web link, G-Motion connects to the server of that link to play it or to create a thumbnail. That server can see your IP address and the usual request details. G-Motion does not control these servers; see their own privacy policies.

## 4. Phone Remote (optional, off by default)

If you turn on the Phone Remote, G-Motion runs a small web server on your computer that only accepts connections from your local network and requires a secret link. Videos you send from your phone are saved on your computer only. Nothing is sent to the developer.

## 5. System information

The System Monitor widget reads CPU, memory, network, and GPU usage from your computer to show it on screen. This information is not stored or sent anywhere.

## 6. Startup

If you turn on "start with Windows", G-Motion registers a Windows startup task. You can turn it off in the app or in Windows Settings > Apps > Startup.

## 7. Sharing and selling data

The developer does not sell your data and does not share it with advertisers. The only services that receive data are the ones listed in section 2 (and the servers of video links you add yourself in section 3).

## 8. Children

G-Motion is not directed at children, and it does not knowingly collect personal information from anyone.

## 9. Your choices

- Turn off the weather features to stop sending location data.
- Uninstall the app at any time; this removes the data it stored on your computer. Videos you sent from your phone are stored in the same place, so back up any you want to keep first.

## 10. Changes to this policy

If this policy changes, the new version will be published at this address with a new "Last updated" date.

## 11. Contact

For questions about this policy, contact the developer through https://github.com/iiRG4.

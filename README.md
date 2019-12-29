# Twilio Phone Client - frontend

This is a web client providing easy access to SMS and call capabilities of a Twilio phone number.

The SMS part is built on top of Twilio's [Programmable Chat API](https://www.twilio.com/docs/chat).

This repository is for the frontend part, it requires [Twilio Phone Client - backend]() for its operation.


## Notable features

 * SMS: Infitinty scolling (older messages get loaded automatically as one scrolls up in a thread)
 * SMS: Hovering over message timestamp displays tooltip with additional details of each message including its SID
 * Configurable accent color (see `REACT_APP_ACCENT_COLOR` in `/.env`)

## Installation

```
npm install
cd deploy; npm install; cd ..
vim deploy/.env  # fill in all the variables
npm run deploy
```

## ToDo

 * Add support for inbound calls (currently only outbound calls are supported)
 * Add support for Multimedia Messages (MMS) for both inbound and outbound
 * Add call history and allow quick redials
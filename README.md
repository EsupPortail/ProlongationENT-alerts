# ProlongationENT-alerts
Simple application displaying alerts (to be used in iframe by ProlongationENT)

## How it works

### Getting alerts

* get the apps (channels) from uPortal/EsupUserApps `/layout`
* displays the apps with "alert_xxx" fnames

### Marking alerts as read

* uses https://github.com/UnivParis1/esup-restdb/

### Is a modal window

This application is meant to be displayed in iframe as a modal window.
* ProlongationENT is taking care of popping this application when there are unread alerts
* to close this application, we send a message to ProlongationENT which will close the modal window (ie remove the iframe)

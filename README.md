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

### Is an iframe

Web components are cool but fragile. ProlongationENT is meant to be used on a many apps (examples: https://github.com/EsupPortail/ProlongationENT-apps) which is quite hard to achieve ([example of issue](https://github.com/EsupPortail/ProlongationENT/commit/b6960746ae44d997a26127dab8a4cccfd1d980ee)). That's why we still use an iframe when possible.

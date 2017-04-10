## Reach boot LED sequence

During boot Reach will go through 3 steps:

* Network scan
* Time sync
* ReachView launch

### Network scan

Reach will indicate a network scan with <font color="yellow">yellow</font> blinks. If a known Wi-Fi network is detected, Reach will connect to it and set the LED <font color="blue">blue</font>. If the scan found no familiar networks, a hotspot is started and the LED will light <font color="green">green</font>.

### Time sync

Time sync is indicated by <font color="magenta">magenta</font> blinks. They are added to the existing networking state indicator. That means that time sync in a hotspot mode will produce <font color="green">green</font>/<font color="magenta">magenta</font> blinks and time sync in a client mode will produce <font color="blue">blue</font>/<font color="magenta">magenta</font> blinks.

### ReachView launch

!!! note
    The app will not launch until the time sync is complete. Internet connection allows this to happen automatically, but in hotspot mode Reach requires a connected antenna with some satellite visibility.

After the time sync is done the <font color="magenta">magenta</font> blinks stop and ReachView will be launched. Successful launch will be signified with a <font color="green">green</font> light, fail will produce a <font color="red">red</font> light.

**More interactive and informative LED statuses will be introduced in one of the future updates.**

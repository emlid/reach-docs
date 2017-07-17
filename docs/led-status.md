## Reach boot LED sequence

Reach LED is an RGB LED that cycles through a simple pattern:

Network state -> App state

During boot Reach will go through 3 steps:

* Network scan
* Time sync
* ReachView launch

### Network scan

During boot, Reach enters a network scan state in which it will try to connect to any known Wi-Fi networks it can find. This might result in connecting to a previously added network or creating its own hotspot.

* Scanning - **fast <font color="blue">blue</font> blinks**
* Client Wi-Fi mode - **<font color="blue">blue</font>**
* Hotspot Wi-Fi mode - **<span style="color: white; background-color: black">white</span>**

### Time sync

After network configuration is done, **<font color="magenta">magenta</font> blinks** will be added to the LED. They are shown during time sync.

### ReachView launch and operation

!!! note
    The app will not launch until the time sync is complete. Internet connection allows this to happen automatically, but in hotspot mode Reach requires a connected antenna with some satellite visibility.

After the time sync is done, the **magenta blinks** stop and ReachView is launched. **<font color="green">Green</font> solid** light will take its place, showing app start. You can see several additional states:

* Normal app operation - **<font color="green">green</font> solid**
* Point collection - **fast <font color="green">green</font> blinks**
* App internal error - **slow <font color="red">red</font> blinks**
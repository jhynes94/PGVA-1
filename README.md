<p align="right">
  <img src="https://user-images.githubusercontent.com/71296226/132049416-fc92dde2-d4fc-4d59-89e9-3aef004c9ee8.png" alt="alt text" width="200" height="30">
</p>

# **PGVA-1**
## **Decentralized Pressure and Vacuum Generator**
<p align="center">
  <img src="https://user-images.githubusercontent.com/71296226/134913029-22fd530b-f09b-4dc2-830f-e82c2f6b2c8f.jpg" alt="alt text" width="750" height="400">
</p>


* Designed to supply [Festo](https://www.festo.com/us/en/?fwacid=9c792b0a20f1ab8d&gclid=Cj0KCQjwm9yJBhDTARIsABKIcGb7XGaLbJ-ljqb2bccWRPNZg1aE6mirUx0hWMCG82ycezodZ9I4ZTgaAqOYEALw_wcB) open-loop pipetting systems and liquid handling systems in the life sciences with compressed air and vacuum.
* The PGVA-1's usage can be extended to other areas as well to aspirate and dispense as a function of the pressure/vacuum levels generated by the PGVA.
* Communication Protocols: [Modbus TCP/IP](https://en.wikipedia.org/wiki/Modbus#Modbus_TCP_frame_format_(primarily_used_on_Ethernet_networks)) and [Modbus Ascii RS232](https://en.wikipedia.org/wiki/Modbus#Modbus_ASCII_frame_format_(primarily_used_on_7-_or_8-bit_asynchronous_serial_lines))

## About
* This is an open software project which provides PGVA-1 customers and users with a wide array of driver templates in different coding languages to allow for quick and easy adaptability of the Festo pressure and vacuum generator to any system, project, or environment. Listed below are the current languages provided along with the methods that each driver provides to the user.

## Links
* [:shopping_cart::Product Page](https://www.festo.com/us/en/e/solutions/industries/life-science/laboratory-automation/in-vitro-diagnostics-id_334908/)
* [:receipt::User Manual](https://www.festo.com/net/SupportPortal/Files/709629/V5_PVGA%20Manual.pdf)
* [:old_key::Support Portal](https://www.festo.com/net/en-gb_gb/SupportPortal/Default.aspx?tab=30&q=8146318)
* [:desktop_computer::GUI](https://www.festo.com/net/en-gb_gb/SupportPortal/Default.aspx?q=8146318&tab=4&s=t#result)

<p align="center">
  <img src="https://user-images.githubusercontent.com/71296226/132046174-046be68a-e6ba-4783-a90b-28b182e50bf7.PNG" alt="alt text" width="500" height="500">
</p>

## Driver Languages
* <img src="https://icons.iconarchive.com/icons/papirus-team/papirus-apps/256/python-icon.png" alt="alt text" width="40" height="40">[  Python](/examples/python)
* <img src="https://images.vexels.com/media/users/3/166401/isolated/lists/b82aa7ac3f736dd78570dd3fa3fa9e24-java-programming-language-icon.png" alt="alt text" width="40" height="40">  [  Java](/examples/java)
* <img src="https://camo.githubusercontent.com/8d56e87edf99e89bfc457cd62462e0b7aae19e6b197b1df5c542d474d8d76f81/68747470733a2f2f646576656c6f7065722e6665646f726170726f6a6563742e6f72672f7374617469632f6c6f676f2f6373686172702e706e67" alt="alt text" width="30" height="30">[  .NET/C#](/examples/c#)

## Methods
* **:syringe: Aspirate** -
  * Purpose:      Aspirates (creates a vacuum) at the given pressure for the given amount of time
  * Value Ranges: actuationTime = 0 to 1000 ms, pressure = -450 to 0 mBar
  * Arguments:    int actuationTime (ms), int pressure (mBar)
  * Returns:      void

* **:droplet: Dispense** -
  * Purpose:      Dispenses (creates an output pressure) at the given pressure for the given amount of time
  * Value Ranges: actuationTime = 0 to 1000 ms, pressure = 0 to 450 mBar
  * Arguments:    int actuationTime (ms), int pressure (mBar)
  * Returns:      void
* **:chart_with_upwards_trend: ReadSensorData** -
  * Purpose:      Reads the actual vaccum, pressure, and output pressure values from the device in mBar
  * Value Ranges: NONE
  * Arguments:    void
  * Returns:      int[] data (data[0] = vacuum, data[1] = pressure, data[2] = output pressure)

### *:radioactive: Advanced Methods*

* **:wrench: Calibration** -
  * Purpose:      Sets the maximum, minimum, and zero pressure set points
  * Value Ranges: NONE
  * Arguments:    void
  * Returns:      void
* **:dash: SetPumpPressure** -
  * Purpose:      Sets pressure and vaccum threshold values in mBar
  * Value Ranges: pressure = 0 to 550 mBar, vacuum = -550 to 0 mBar
  * Arguments:    int pressure (mBar), int vacuum (ms)
  * Returns:      void

## Contributors
|Name                 | Email                         | GitHub         |
| ------------        | -------------------------     | -------------- |
| John Alessio        | alessio.j@northeastern.edu    | @jalesssio     |
| Justin Hynes-Bruell | justin.hynes-bruell@festo.com | @jhynes94      |
| Milen Kolev         | milen.kolev@festo.com         | @MKollev       |
| Jared Raines        | raines.j@northeastern.edu     | @rainesjared   |

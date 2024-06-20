# ESP32-S3-Box3-IR-Blaster-Learning-Example

This is a learning example for the ESP32 S3 Box3
Shows how to enable the IR receiver (`remote_receiver`), read the input, run (currently very simple) logic to learn the signal, and then blast the signal through the IR diode (`remote_transmitter`).

## Usage
On the Status screen:
 - push the top left physical button to enter IR Learning Mode
 - push the physical mute button to send an IR broadcast (if one has been learned)

On the IR Learning screen, click any IR button toward the IR receiver several times over the alotted time to learn the signal.

## Notes

In my experience, the IR diode in the S3 Box3 sensor dock was not very powerful, failing to transmit to my TV which was 2.3m away from the sensor dock.  At 1.4m it worked reliably.  To test your ir transmissions, you can enable the IR receiver while on the Status screen and then transmit with the Mute button.  You'll see any received data in the logs.

# Windows Setup

1. Install Android Platform Tools from the official Android developer distribution.
2. Install the appropriate USB driver if Windows does not recognize the device.
3. Connect the phone using a data-capable USB cable.
4. Enable USB debugging only when needed.
5. Run `adb devices` and approve the authorization prompt on the phone.
6. Verify Fastboot separately with `fastboot devices`.

Record the Windows version, driver package/version and Platform Tools version in your own test log.

# Transceiver KiwiSDR Bridge User Guide

Version: 1.1.20  
Author: John Burns, GW3JVB

## What It Does

Transceiver KiwiSDR Bridge links a supported radio or SDR program to a KiwiSDR browser page. When you tune the radio VFO or change mode, the KiwiSDR page follows.

## Supported Radio Options

- Icom IC-7300 using CI-V serial
- TCI Protocol using network TCI, including Thetis, Expert Electronics, Apache Labs ANAN, and Hermes Lite 2 where TCI is available
- Yaesu FT-920(R) experimental using serial CAT
- Yaesu FTDX10 experimental using Yaesu CAT over the Enhanced USB COM port
- Hamlib using the bundled Hamlib support

## Installation

1. Download the latest installer from the Releases page:

   <https://github.com/reflectingme/TransceiverKiwiSDRBridge-Downloads/releases>

2. Run the installer:

   ```text
   Transceiver-KiwiSDR-Bridge-Setup-vX.X.X.exe
   ```

3. Follow the setup pages.

4. Start Transceiver KiwiSDR Bridge from the desktop shortcut or Start menu.

## Browser Extension Setup

The app uses a local browser extension so it can control the KiwiSDR web page.

You must load the included extension folder into the browser you want to use.

### Chrome

1. Open Chrome.
2. Enter this in the address bar:

   ```text
   chrome://extensions/
   ```

3. Turn on **Developer mode**.
4. Click **Load unpacked**.
5. Select the extension folder installed with the app.

### Brave

1. Open Brave.
2. Enter this in the address bar:

   ```text
   brave://extensions/
   ```

3. Turn on **Developer mode**.
4. Click **Load unpacked**.
5. Select the extension folder installed with the app.

### Microsoft Edge

1. Open Edge.
2. Enter this in the address bar:

   ```text
   edge://extensions/
   ```

3. Turn on **Developer mode**.
4. Click **Load unpacked**.
5. Select the extension folder installed with the app.

## Finding The Extension Folder

In the app, use **Copy Folder Path** to copy the correct extension folder path to the clipboard.

When the browser asks which folder to load, paste or browse to that folder.

Do not select the main app folder. Select the folder named:

```text
extension
```

## Basic Use

1. Open Transceiver KiwiSDR Bridge.
2. Click **Settings**.
3. Select your radio type.
4. Enter or select the correct radio connection details.
5. Enter the KiwiSDR host and port.
6. Select the browser you configured.
7. Click **Save**.
8. Click **Start Bridge**.
9. Open the KiwiSDR page.
10. Tune the radio VFO or change mode.

The KiwiSDR page should follow the connected radio.

## Common Settings

### Icom IC-7300

- Baud rate: `115200`
- CI-V address: `94`
- Serial port: select the COM port shown in Windows Device Manager

### TCI Protocol

- TCI host: IP address or host name of the computer, radio, or SDR application providing TCI
- TCI port: usually `50001`

### KiwiSDR

Example:

```text
Host: g3sdr.com
Port: 8077
```

You may also paste a full KiwiSDR URL, for example:

```text
http://radio.satelliteboy.com:8073/
```

The app will store the host and port separately.

Previously used KiwiSDR hosts can be selected from the host dropdown.

## Common Problems

### The browser extension does not appear

Check that Developer mode is enabled and that you selected the `extension` folder.

### The app starts but KiwiSDR does not follow

Check that:

- The bridge is started.
- The browser extension is installed in the selected browser.
- The KiwiSDR page is open in that selected browser.
- The selected radio type and port settings are correct.

### The wrong COM port is selected

Open Windows Device Manager and check **Ports (COM & LPT)**.

## Support

- App page: <https://gw3jvb.uk/transceiver-kiwisdr-bridge/>
- Discord: <https://discord.gg/yTW4DzBBKQ>
- Email: <mailto:gw3jvb@gmail.com>

If you find the app useful and would like to support future development:

- PayPal: <https://www.paypal.com/paypalme/JohnVincentBurns>
- Buy Me a Coffee: <https://buymeacoffee.com/reflectingme>

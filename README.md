# i3bar Configuration File

## Description

This repository contains the configuration file (`i3status.conf`) for i3bar, used in conjunction with the i3 window manager (i3wm). The configuration sets up various system information to be displayed in the i3bar, including load, memory usage, CPU temperature, battery status, and local time. Additionally, it uses NerdFonts for enhanced iconography.

## Configuration Details

### General Settings

- **Colors**: Disabled (`colors = false`)
- **Update Interval**: 10 seconds

### Modules Displayed

- **Load**: Displays system load.
- **Memory**: Shows memory usage.
- **CPU Temperature**: Displays the CPU temperature.
- **Battery**: Shows battery status and percentage.
- **Local Time**: Displays current time and date.

### CPU Temperature Path Consistency

To ensure the CPU temperature folder path is consistent across reboots, follow the guide provided at [joonas.fi](https://joonas.fi/2021/07/stable-device-path-for-linux-hwmon-interfaces/).

### Fonts

This configuration uses NerdFonts for enhanced iconography. Make sure to have NerdFonts installed on your system.

## Installation

### Prerequisites

- i3 window manager
- [NerdFonts](https://www.nerdfonts.com/)

### Steps

1. **Clone the Repository**: Clone this repository to your local machine.
   ```bash
   git clone https://github.com/xHardc0re/i3bar-config.git
   ```

2. **Create Configuration Directory**: Ensure the i3status configuration directory exists.
   ```bash
   mkdir -p ~/.config/i3status
   ```

3. **Copy Configuration File**: Copy the `i3status.conf` file to the configuration directory.
   ```bash
   cp i3bar-config/i3status.conf ~/.config/i3status/
   ```

4. **Set Up CPU Temperature Path**: Follow the guide at [joonas.fi](https://joonas.fi/2021/07/stable-device-path-for-linux-hwmon-interfaces/) to make the CPU temperature folder path consistent across reboots.

5. **Install NerdFonts**: Ensure NerdFonts are installed on your system.

6. **Reload i3wm Configuration**: Reload your i3wm configuration to apply the changes.
   ```bash
   $mod+Shift+r
   ```

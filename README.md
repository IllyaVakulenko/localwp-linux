# Installing Local WP on Ubuntu

This guide will help you set up Local WP on Ubuntu, including resolving dependency issues that may occur during installation.

## Prerequisites
- Ubuntu 20.04 or newer
- Administrator access to install required packages

---

## Installation Steps

### Step 1: Download and Install Dependencies
Local WP requires several additional libraries to run on Ubuntu. Follow the steps below to install these dependencies manually:

1. **Install `libtinfo5`**  
   Download and install the `libtinfo5` package:
   ```bash
   curl -O http://launchpadlibrarian.net/648013231/libtinfo5_6.4-2_amd64.deb
   sudo dpkg -i libtinfo5_6.4-2_amd64.deb
   ```

2. **Install `libncurses5`**
   Download and install the `libncurses5` package:
   ```bash
   curl -O http://launchpadlibrarian.net/648013227/libncurses5_6.4-2_amd64.deb
   sudo dpkg -i libncurses5_6.4-2_amd64.deb
   ```

3. **Install `libaio1`**
   Download and install the `libaio1` package:
   ```bash
   curl -O http://launchpadlibrarian.net/646633572/libaio1_0.3.113-4_amd64.deb
   sudo dpkg -i libaio1_0.3.113-4_amd64.deb
   ```

4. **Install `libnss3-tools`**
   Use the following command to install `libnss3-tools` via apt:
   ```bash
   sudo apt install libnss3-tools
   ```

---

## Step 2: Download Local WP

Visit the official [Local WP](https://localwp.com/) download page and download the latest Linux version of the application.

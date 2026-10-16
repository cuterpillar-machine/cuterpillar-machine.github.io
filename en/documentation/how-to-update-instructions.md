---
layout: documentation
ref: how-to-update
title: How to Update Instructions
description: How to update the Cuterpillar machine firmware over Wi-Fi (OTA) from a browser.
---

The firmware is updated over Wi-Fi right from your browser, no USB cable needed.

## What to download

On the [Versions page]({{ '/en/versions.html' | relative_url }}), download the files of the release you need:

- `firmware.bin`: the firmware itself;
- `littlefs.bin`: the machine's web interface.

Update both files together: the firmware and the web interface must be the same version.

## Update steps

1. **Wait for the job to finish.** While the machine is cutting or homing, the update button is disabled.
2. **Open the machine's web interface:**
   - on home Wi-Fi: `http://cut.local`, or the IP address shown on the machine's display;
   - in direct connection mode: join the `Cuterpillar-XXXX` network and open `http://192.168.4.1`.
3. **Tap "Update Firmware".** The update page opens.
4. **Upload `firmware.bin`.** The machine reboots by itself when the upload finishes.
5. **Open the update page again and upload `littlefs.bin`.** The machine reboots again.

Some office and guest networks block the `cut.local` address. Use the IP address from the display instead.

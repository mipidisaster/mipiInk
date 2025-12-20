# mipiInk
Full project, containing the complete suite of artefacts to generate the mipiInk setup/system.

```mermaid
gitGraph
commit id: "v0.0.0"
commit id: "v0.1.0"
commit id: "v1.0.0"
```

## v1.0.0
Step up in the project;
1. Running `server\server.py` on local machine (Windows tested, but intended for RaspberryPi/Linux) will create a webpage at the IP address:5000. In this webpage files (specifically images) can be uploaded onto the server, and then pushed to the eInk/Pico display
2. Pico needs to be running at the same time, and run `device/pico-WiFi.py`

Note, at the root of the pico there needs to be a file called `private_keys` with parameters:
- ssid
- password

> Note, issue on the image brightness has been reported; [Issue #2](https://github.com/mipidisaster/mipiInk/issues/2)

> Note2, Also due to a SD Card/eInk display interaction issue, please disconnect the eInk on power-up, run `device/pico-WiFi.py` (confirming that the SD Card is indeed read), then exit "ctrl+c".
Reconnect the eInk display, and re-run, you should again see the SD card as being read. If not, please update [Issue #7](https://github.com/mipidisaster/mipiInk/issues/7)

### Problems worked
- [Issue #3](https://github.com/mipidisaster/mipiInk/issues/3)
- [Issue #6](https://github.com/mipidisaster/mipiInk/issues/6)
- [Issue #8](https://github.com/mipidisaster/mipiInk/issues/8)
- [Issue #9](https://github.com/mipidisaster/mipiInk/issues/9)
- [Issue #10](https://github.com/mipidisaster/mipiInk/issues/10)
- [Issue #11](https://github.com/mipidisaster/mipiInk/issues/11)

### Limitations
Nether device has any protection for none images being converted and/or pushed to the eInk/Pico, so only use .jpg or .png when sending to the eInk/Pico.
Recorded as [Issue #19](https://github.com/mipidisaster/mipiInk/issues/19)

# Support
> Any other issues, record within [mipidisaster/mipiInk.Software](https://github.com/mipidisaster/mipiInk.Software)

or hardware issues, record within [mipidisaster/mipiInk.Electronics](https://github.com/mipidisaster/mipiInk.Electronics)
# mipiInk
Full project, containing the complete suite of artefacts to generate the mipiInk setup/system.

```mermaid
gitGraph
commit id: "v0.0.0"
commit id: "v0.1.0"
```

## v0.1.0
Initial "Minimum Viable Product"; basic interface to a single supported eInk display. Mechanism to upload image:
1. Copy desired image into `Software/server/images", naming it `testImage.jpg` (any other name would require a change to code)
2. Run the `process_image.py` scipt on local machine; which will generate a `testImage-preprocessed.bin` at `Software/server/`
3. Copy this image onto SDcard (at root level)
4. Connect SDcard to prototype breadboard
5. Connect pico to computer, and then run `device/main-pico.py`

> If errors, then ensure that scripts `ePaper5_65.py` and `lib/sdcard.py` are both in the pico root directory

> Any other issues, record within [mipidisaster/mipiInk.Software](https://github.com/mipidisaster/mipiInk.Software)
    
8. Image should then appear on the eInk

> Note, issue on the image brightness has been reported; [Issue #2](https://github.com/mipidisaster/mipiInk/issues/2)
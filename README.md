# esp32_free_cat_wifi
Use esp32 to serve free wifi with cats.

## Installing esp-idf

- Follow the instructions here: https://docs.espressif.com/projects/esp-idf/en/stable/esp32/get-started/linux-macos-setup.html#

## Building, Flashing, and Monitoring
- esp-idf$ . ./export.sh
- esp32_free_cat_wifi$ idf.py set-target esp32
- esp32_free_cat_wifi$ idf.py build
- esp32_free_cat_wifi$ idf.py flash
- esp32_free_cat_wifi$ idf.py monitor
  - To exit IDF monitor use the shortcut Ctrl+].

## Adding cats
Cats (images) need to be added manually.
- mkdir cats
- Put .jpg images of cats in the newly created cats-folder.
  - Name them catX.jpg, where X is 0, 1, 2, ...
  - Make sure the images are quite small. The filesystem has a very limited 1M of space.
- Update NUM_CATS macro in main.c.

## Hardware
ESP32-WROOM-32 DevKit LiPo

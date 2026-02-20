idf_component_register(SRCS main.c
                       PRIV_REQUIRES esp_event nvs_flash esp_wifi esp_http_server dns_server)

littlefs_create_partition_image(storage ../cats FLASH_IN_PROJECT)

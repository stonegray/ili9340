
set(COMPONENT_SRCS
    driver/decode_image.c
    driver/fontx.c
    driver/ili9340.c
    driver/pngle.c
)

set(COMPONENT_ADD_INCLUDEDIRS
    driver/include
)
register_component()
    
spiffs_create_partition_image(storage font FLASH_IN_PROJECT)

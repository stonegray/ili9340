
set(COMPONENT_SRCS
    decode_image.c
    fontx.c
    ili9340.c
    pngle.c
)

set(COMPONENT_ADD_INCLUDEDIRS . )

register_component(REQUIRES driver)
    
#spiffs_create_partition_image(storage font FLASH_IN_PROJECT)




set(COMPONENT_SRCS
    decode_image.c
    fontx.c
    ili9340.c
    pngle.c
)

set(COMPONENT_ADD_INCLUDEDIRS . )

idf_component_register(SRCS ${COMPONENT_SRCS}
                  INCLUDE_DIRS ${COMPONENT_ADD_INCLUDEDIRS}
                  REQUIRES driver)
#idf_component_register(PRIV_REQUIRES driver SRCS "src/esp_dmx.c" INCLUDE_DIRS "src/" "src/dmx")   
#spiffs_create_partition_image(storage font FLASH_IN_PROJECT)

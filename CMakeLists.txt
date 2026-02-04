if(ESP_PLATFORM)
    set(srcs
        "esp32_dht.c")

    set(includes 
        ".")

    set(requires
        esp_driver_gpio)

    idf_component_register(SRCS "${srcs}"
                           INCLUDE_DIRS ${includes}
                           REQUIRES ${requires})
endif()

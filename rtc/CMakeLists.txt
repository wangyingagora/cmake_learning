set(LIBRARY_OUTPUT_PATH ${PROJECT_BINARY_DIR}/lib)

set(RTC_SRC rtc.c)
add_library(rtc SHARED ${RTC_SRC})
add_library(rtc_static STATIC ${RTC_SRC})

set_target_properties(rtc PROPERTIES CLEAN_DIRECT_OUTPUT 1)
set_target_properties(rtc_static PROPERTIES OUTPUT_NAME "rtc")

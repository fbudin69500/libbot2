add_executable(bot-lcm-logfilter
    lcm-logfilter.c)
set_property(TARGET bot-lcm-logfilter PROPERTY C_STANDARD 99)
target_link_libraries(bot-lcm-logfilter ${lcm_namespace}lcm GLib2::glib)

pods_install_executables(EXPORT ${POD_NAME} bot-lcm-logfilter)

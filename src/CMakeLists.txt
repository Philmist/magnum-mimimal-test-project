find_package(Magnum REQUIRED
    Sdl2Application)

find_package(sdl2 REQUIRED
    Sdl2Application)

set_directory_properties(PROPERTIES CORRADE_USE_PEDANTIC_FLAGS ON)

add_executable(MyApplication MyApplication.cpp)
target_link_libraries(MyApplication PRIVATE
    Magnum::Application
    Magnum::Magnum
    SDL2::SDL2)

set (idiff_srcs idiff.cpp)
add_executable (idiff ${idiff_srcs})
set_target_properties (idiff PROPERTIES FOLDER "Tools")
target_link_libraries (idiff OpenImageIO ${Boost_LIBRARIES} ${CMAKE_DL_LIBS})
link_ilmbase (idiff)
oiio_install_targets (idiff)

set( EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_BINARY_DIR} )

add_executable( abstractgridtest abstractgridtest.cpp ../src/abstractgrid.cpp )
add_test(abstractgridtest abstractgridtest)
ecm_mark_as_test(abstractgridtest)
target_link_libraries( abstractgridtest Qt5::Gui Qt5::Test KF5::XmlGui)

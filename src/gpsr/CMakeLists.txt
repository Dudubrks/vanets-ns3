build_lib(
  LIBNAME gpsr
    SOURCE_FILES
    model/gpsr-ptable.cc
    model/gpsr-rqueue.cc
    model/gpsr-packet.cc
    model/gpsr.cc
    helper/gpsr-helper.cc
  HEADER_FILES
    model/gpsr-ptable.h
    model/gpsr-rqueue.h
    model/gpsr-packet.h
    model/gpsr.h
    helper/gpsr-helper.h
  LIBRARIES_TO_LINK ${libinternet}
                    ${libwifi}
  TEST_SOURCES
    test/gpsr-test-suite.cc
)

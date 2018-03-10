FIND_PATH(myHeader hello.h)
IF(myHeader)
INCLUDE_DIRECTORIES(${myHeader})
ENDIF(myHeader)

LINK_DIRECTORIES( /tmp/t3/usr/lib/)
ADD_EXECUTABLE(main main.c)
TARGET_LINK_LIBRARIES(main libhello.a)

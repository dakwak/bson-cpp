# add sources
SET(SOURCES
  ../lib/base64.cpp
  oid.cpp
  bsonobj.cpp
  util/json.cpp
  ../lib/md5.c
  ../lib/nonce.cpp
  )

# the executable
ADD_LIBRARY(${PROJECT_NAME} SHARED ${SOURCES})
INSTALL(TARGETS ${PROJECT_NAME} LIBRARY DESTINATION lib)

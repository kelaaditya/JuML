FILE(GLOB CLASSIFICATION_SRC *.cpp)
ADD_LIBRARY(classification SHARED ${CLASSIFICATION_SRC})
TARGET_LINK_LIBRARIES(classification ${AF_LIBS} core data preprocessing)

# Test for K_MEANS
ADD_EXECUTABLE(KMEANS_TEST KMeans.cpp)
TARGET_LINK_LIBRARIES(KMEANS_TEST core clustering gtest gtest_main ${CMAKE_THREAD_LIBS_INIT})
ADD_MPI_TEST(KMEANS_TEST KMEANS_TEST 1 2 5 8)

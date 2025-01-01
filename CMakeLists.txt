cmake_minimum_required(VERSION 3.10)
project(VulkanWindowTest)

set(CMAKE_CXX_STANDARD 17)

# Подключение библиотек Vulkan и GLFW
find_package(Vulkan REQUIRED)
find_package(glfw3 3.3 REQUIRED)

# Указание исходных файлов
add_executable(VulkanWindowTest src/main.cpp)

# Линковка с Vulkan и GLFW
target_link_libraries(VulkanWindowTest Vulkan::Vulkan glfw)

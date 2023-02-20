cmake_minimum_required(VERSION 3.0.2)
project(zero100_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_filters
  message_generation
  std_msgs
)

## Generate messages in the 'msg' folder
add_message_files(
   FILES
   Heading.msg
)


## Generate added messages and services with any dependencies listed here
generate_messages(
   DEPENDENCIES
   std_msgs
)


catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES zero100_msgs
#  CATKIN_DEPENDS message_filter message_generation std_msgs
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)


## Add folders to be run by python nosetests
# catkin_add_nosetests(test)

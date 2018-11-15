cmake_minimum_required(VERSION 2.8.3)
project(bmt_bu_sw_msgs)

find_package(catkin REQUIRED COMPONENTS
  message_generation
  std_msgs
)

################################################
## Declare ROS messages, services and actions ##
################################################


## Messages in the 'msg' folder
 add_message_files(
   FILES
   IMUData.msg
 )

## Services in the 'srv' folder
# add_service_files(
#   FILES
#   Service1.srv
#   Service2.srv
# )

## Actions in the 'action' folder
# add_action_files(
#   FILES
#   Action1.action
#   Action2.action
# )

## Generate added messages and services with any dependencies listed here
 generate_messages(
   DEPENDENCIES
   std_msgs
 )

################################################
## Declare ROS dynamic reconfigure parameters ##
################################################

###################################
## catkin specific configuration ##
###################################
catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES bmt_bu_sw_msgs
  CATKIN_DEPENDS std_msgs
)

###########
## Build ##
###########

#############
## Install ##
#############

#############
## Testing ##
#############


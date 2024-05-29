cmake_minimum_required(VERSION 3.20.0)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

project(BMA456-example)

# target_sources(app PRIVATE src/motion.c)
# target_sources(app PRIVATE src/activity.c)
target_sources(app PRIVATE src/step_counter.c)

target_sources(app PRIVATE src/bma4.c)
target_sources(app PRIVATE src/bma456w.c)
target_sources(app PRIVATE src/common.c)

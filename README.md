# rcl_logging_rcutils

This repo is an `rcl_logging` implementation using the `rcutils` logger.
It logs to stderr (by default) without touching the file system.
This idea is to enable logging on read-only filesystems.
The default `rcl_logging_spdlog` can't be used because it errors if it can't create a directory in `ROS_HOME`.

If you came here becase you need a logger on Android, see [`rcl_logging_android`](https://github.com/sloretz/rcl_logging_android).

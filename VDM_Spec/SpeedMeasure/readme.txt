The default time step in the simulator is 1 nsec. However, in the current release (Overture 1.0), the time base for periodic threads is 1 msec. So, specifying periodic(2000,0,0,0) would yield a 2 second time interval, which is shown as 2000000000 in the log file viewer. Furthermore, this implicates that you cannot define periodic tasks that run faster than 1 kHz.

In the upcoming Overture 1.1 release, this will be corrected and all time units (in periodic and duration) refer to the same (unified) 1 nsec time step.

Currently, it is not possible to change the time step size in the simulator.
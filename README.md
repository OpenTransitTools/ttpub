The _TimeTablePublisher _ is a single system that allows a transit agency to examine, modify, and transform raw scheduling data into easy-to-read timetables for customer information purposes.  The application simplifies and accelerates the production of printed on-street schedules and web schedules, which is often a very time-consuming and manual process for most agencies.  This results in more accurate, current, and consistent schedule information for the customer.


The TimeTablePublisher is designed to use data directly in the [http://code.google.com/transit/spec/transit_feed_specification.html Google Transit Feed Spec (GTFS)] format, so it can be very easy for an agency to implement.  In addition, it can connect to, and read from, other sources of data including a database, a comma separated text file, and XML.  An easy-to-use interface, as well as a tool that compares the changes between two service dates, makes it easy to format and edit the data.


As an open sources application, TimeTablePublisher is available for free so that other transit agencies can use it and even contribute enhancements to it.  There's always room for improvement; and with your help, TimeTablePublisher will improve.


------------
SUGGESTIONS:

1. Use the war file (look right).  Just drop it into your TOMCAT/webapps directory.  It will unpack itself, and you should see a TOMCAT/webapps/ttpub directory (assuming tomcat is running).

2. Use the test GTFS data (again, look right).  This data-set very is small, and thus provides a good sanity check that TimeTablePublisher (TTPUB) is properly configured on your machine.

3. It's been reported that 512 megs is just not enough memory to run TTPUB with real schedule data.  GTFS data is really big, and TTPUB is really bad at memory management.  The minimum memory on your system should be 1.5 GB -- you're recommended to be dedicating 1G (eg: JAVA_OPTS="-Xmx1024m") of memory to TTPUB.

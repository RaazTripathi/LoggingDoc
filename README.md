LoggingDoc
==========
A simple Log4j file .











## --------------------------------------------------
## ROOT APPENDER USED BY EYOGABASE
## --------------------------------------------------
log4j.rootCategory=INFO, Stdout, eYogaBaseLogFile
#
## --------------------------------------------------
## Basic Console Appender
## --------------------------------------------------
log4j.appender.Stdout=org.apache.log4j.ConsoleAppender
log4j.appender.Stdout.Threshold=DEBUG
log4j.appender.Stdout.layout=org.apache.log4j.PatternLayout
log4j.appender.Stdout.layout.ConversionPattern=%d %-5p %t [%c] %m%n

## --------------------------------------------------
## Rolling Log File Appender
## --------------------------------------------------
log4j.appender.eYogaBaseLogFile=org.apache.log4j.RollingFileAppender
log4j.appender.eYogaBaseLogFile.Threshold=TRACE
log4j.appender.eYogaBaseLogFile.MaxFileSize=1024KB
log4j.appender.eYogaBaseLogFile.MaxBackupIndex=10
log4j.appender.eYogaBaseLogFile.layout=org.apache.log4j.PatternLayout
log4j.appender.eYogaBaseLogFile.layout.ConversionPattern=%d %-5p %t [%c{3}] %m%n
log4j.appender.eYogaBaseLogFile.File=C:/Program Files/Apache Software Foundation/Tomcat 6.0/logs/eyogabase.log
#
## ---------------------------------------------
#log4j.logger.org.apache.catalina=debug
#log4j.logger.org.apache.struts2=debug
#log4j.logger.org.apache.tiles=debug
#log4j.logger.com.opensymphony.xwork2=debug
#log4j.logger.org.springframework.jdbc=debug

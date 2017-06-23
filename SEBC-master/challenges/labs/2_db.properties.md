$cat /var/log/cloudera-scm-server/cloudera-scm-server.log|head -1

2017-06-23 03:53:02,748 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.10.0 (#85 built by jenkins on 20170120-1037 git: aa0b5cd5eceaefe2f971c13ab657020d96bb842a)


$grep -n "Started Jetty server" /var/log/cloudera-scm-server/cloudera-scm-server.log

31170:2017-06-23 03:54:13,637 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.

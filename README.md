ktop
====

Karaf Top Command

 ktop - display and update sorted information about JVM and threads.

Description:

 The ktop command displays key JVM metrics, and updates a sorted list
 of thread statistics. 

Building from source:
===

To build, invoke:
```
mvn install
```

Bundle-Install
===

To install in Karaf, invoke from console:
```
install -s mvn:com.savoirtech.karaf.commands/ktop
```
specify version if needed
```
install -s mvn:com.savoirtech.karaf.commands/ktop/0.3.0-SNAPSHOT
```

uninstall
```
uninstall <bundle-id>
```

Alternative Feature-Install
===

```
feature:repo-add mvn:com.savoirtech.karaf.commands/ktop/0.3.0-SNAPSHOT/xml/features
feature:install -v ktop
```

uninstall
```
feature:uninstall ktop
feature:repo-remove mvn:com.savoirtech.karaf.commands/ktop/0.3.0-SNAPSHOT/xml/features
```


To execute command on Karaf, invoke:
```
aetos:ktop
```

To exit ktop: q
To sort by a different column: < or >
To reverse sort: r


Runtime Options:
===

 -t  --threads   number of threads to display. 
 -u  --updates   information update interval in milliseconds.

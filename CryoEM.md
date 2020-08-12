Cryo EM data egress testing via perfSONAR


Optionally lookup SDSC perfSONAR nodes via

http://stats.es.net/ServicesDirectory/

Log on to a server that has pScheduler (MiServer uses main Umich password)

```
ssh perfsonar.miserver.it.umich.edu
```


Traceroute from CryoEM pS node to SDSC:

```
pscheduler task trace \
  --source=test10g.lsi.umich.edu \
  --dest=ps.sdsc.xsede.org
```

Latency

```
pscheduler task latency \
  --source=test10g.lsi.umich.edu \
  --dest=ps.sdsc.xsede.org
```

Throughput

```
pscheduler task throughput
  --source=test10g.lsi.umich.edu \
  --dest=ps.sdsc.xsede.org
```

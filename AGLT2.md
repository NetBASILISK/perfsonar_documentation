Cryo EM data egress testing via perfSONAR


First lookup SDSC perfSONAR nodes via

http://stats.es.net/ServicesDirectory/

Log on to a server that has pScheduler (MiServer uses main Umich password)

```
ssh perfsonar.miserver.it.umich.edu
```


Traceroute from CryoEM pS node to SDSC:

```
pscheduler task trace \
  —-dest=psum02.aglt2.org \
  —-source=lhcmon.bnl.gov 
```

Latency

```
pscheduler task latency \
  —-dest=psum02.aglt2.org \
  —-source=lhcmon.bnl.gov 
```

Throughput

```
pscheduler task throughput
  —-dest=psum02.aglt2.org \
  —-source=lhcmon.bnl.gov 
```

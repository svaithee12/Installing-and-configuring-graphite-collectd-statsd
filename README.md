# Installing-and-configuring-graphite-collectd-statsd
This repository contains the documentation to install and configure graphite, collectd and statsd .

install graphite.
install collectd at server and at client and configure.
install tail plugin at client.


1. Collectd collects data from its plugins and writes to graphite using the write_graphite plugin.

2. StatsD is event counter/aggregation service. It receives per-event timings and calculates and generates aggregated values. It is built to count/aggregate custom applications metrics. It only requires the application to send events, without any need for aggregations.

3. The statsd plugin of collectd is collectd data FROM statsd.
and is explained in the link : https://anomaly.io/statsd-in-collectd/

4. StatsD could be used to aggregate events from services which can then be fed to CollectD. (CollectD can then fed it Graphite) But CollectD in itself has plugins to collect stats from services as well.

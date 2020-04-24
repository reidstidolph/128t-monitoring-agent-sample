# 128t-monitoring-agent-sample
This contains a sample of output data produced by the 128T monitoring agent. The `sample.json` contained in this repo is from a production router monitoring agent using the following configuration:
```
enabled: true
tags:
- key: router
  value: ${ROUTER}
sample-interval: 5
push-interval: 300
inputs:
- name: t128_events
- name: t128_metrics
- name: t128_device_state
- name: t128_peer_path
outputs:
- name: file
```
That is sampling data every 5 seconds, and the `sample.json` contains a data set which pushed at the 300 second interval.

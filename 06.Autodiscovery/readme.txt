  - job_name: 'data'
    file_sd_configs:
    - files:
      - '/etc/prom-targets/*.json'
      refresh_interval: 5s

root@prometheus:~# cat /etc/prom-targets/dd.json 
[
        {
                "targets": [
                        "192.168.0.100:9100",
                        "192.168.0.200:9100"
                ],
                "labels": {
                        "env": "dev"
                }
        }
]


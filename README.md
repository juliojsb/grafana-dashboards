# Grafana Dashboards

A collection of my Grafana dashboards.

## MySQL/MariaDB Statistics

* *Description:* MySQL usage statistics like number of connections, cache size, query cache, locks... and general system resources (CPU, memory, network)
* *Metric collector:* collectd
* *Plugins:* mysql, cpu, ram, upload, network. Information about the configuration in my [blog](https://www.elarraydejota.com/dashboard-mysql-mariadb-en-grafana-collectd)
* Screenshots:

![grafana1](https://user-images.githubusercontent.com/12804701/57197612-c2aede00-6f69-11e9-848f-284514dafa2f.png)
![grafana2](https://user-images.githubusercontent.com/12804701/57197613-c478a180-6f69-11e9-9e46-e5e5f8a6e597.png)
![grafana3](https://user-images.githubusercontent.com/12804701/57197614-c5a9ce80-6f69-11e9-8b91-3bb5c1b0e41c.png)
![grafana4](https://user-images.githubusercontent.com/12804701/57197615-c6426500-6f69-11e9-9793-d2f00345e34d.png)


## CPU & Nvidia Graphic Card

* *Description:* detailed CPU usage, including CPU modes, frequency and temperature (per core and global)
* *Metric collector:* collectd
* *Plugins:* cpu, cpufreq, exec. For the exec plugin I use [collectd-cuda](https://github.com/kwilczek/collectd-cuda) which gives Nvidia Graphic Card data (temperature, fan speed, memory usage...)
* Screenshots:

![grafana_cpu_usage](https://user-images.githubusercontent.com/12804701/57197603-b1fe6800-6f69-11e9-9679-b30af201964f.png)
![nvidia_graphic_card](https://user-images.githubusercontent.com/12804701/57197601-af9c0e00-6f69-11e9-8f29-1e9c0986085a.png)


## Basic Security

* *Description:* basic security information like number of hits by mod_security, SSH failed connections, fail2ban blocks...
* *Metric collector:* collectd
* *Plugins:* tail. Information about the configuration in my [blog](https://www.elarraydejota.com/metricas-de-seguridad-con-plugin-tail-de-collectd-y-dashboard-en-grafana)
* Screenshots:

![grafana_modsecurity_blocks](https://user-images.githubusercontent.com/12804701/57197630-f38f1300-6f69-11e9-8c59-5dd5f3ae3609.png)
![total_user_sessions](https://user-images.githubusercontent.com/12804701/57197631-f4c04000-6f69-11e9-9db4-b9b9509f48b7.png)
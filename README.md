Antifilter routes installer
===========================

### Description
This is ansible role for install the script, which will download list of IPs, forbidded by RKN in Russia.
Also it contains [script](https://github.com/phoenix-mstu/net_list_minimizer) from [Grigory Kuzovnikov](https://github.com/phoenix-mstu) for minimize count of prefixes.

### Defaults
```
rkn_dir: /opt/rkn
net_minimizer_dir: /opt/net_list_minimizer
prefix_count: 3000
rkn_tpl:
  - src: 'makeroutes.sh.j2'
    dst: "{{ rkn_dir }}/makeroutes.sh"
    mode: '0755'
```

### Limitations
No any guarantees. All at your own risk.
Author is not responsible for the content of files, placed on the [antifilter.download](antifilter.download)

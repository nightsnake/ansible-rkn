Antifilter routes installer
===========================

### Description
This is ansible role for install the script, which will download list of IPs, forbidded by RKN in Russia.

### Defaults
```
rkn_dir: /opt/rkn
rkn_tpl:
  - src: 'makeroutes.sh.j2'
    dst: "{{ rkn_dir }}/makeroutes.sh"
    mode: '0755'
```

### Limitations
No any guarantees. All at your own risk.
Author is not responsible for the content of files, placed on the [antifilter.download](antifilter.download)

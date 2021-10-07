# Prometheus host base monitoring

## Node exporter
1. Download `node-exporter` and move to `/usr/bin`
2. Create `node-exporter.service` into `/etc/systemd/system`
3. Create `node-exporter` user
```shell
useradd --system node_exporter
```
4. Start `node-exporter`
```shell
systemctl daemon-reload
systemctl enable node-exporter
systemctl start node-exporter
```
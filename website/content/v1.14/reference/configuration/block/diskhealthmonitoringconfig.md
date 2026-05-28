---
description: |
    DiskHealthMonitoringConfig is a disk health monitoring configuration document.
    Configures periodic disk health monitoring. When enabled, Talos collects
    passive health information from NVMe and ATA disks and publishes
    DiskHealthStatus resources.
title: DiskHealthMonitoringConfig
---

<!-- markdownlint-disable -->



{{< highlight yaml >}}
apiVersion: v1alpha1
kind: DiskHealthMonitoringConfig
enabled: true # Enable or disable disk health monitoring.
interval: 5m # Polling interval for disk health checks.
{{< /highlight >}}


| Field | Type | Description | Value(s) |
|-------|------|-------------|----------|
|`enabled` |bool |Enable or disable disk health monitoring.  |`true`<br>`false`<br> |
|`interval` |string |Polling interval for disk health checks.<br>Must be a valid Go duration string (e.g. "5m", "30s", "1h").  | |

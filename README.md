# windows-exporter-dashboard-custom

Import the Following Json Dashboard in Your Grafana Dasboard 
Manage => import => json section
```
{
  "annotations": {
    "list": [
      {
        "builtIn": 1,
        "datasource": "-- Grafana --",
        "enable": true,
        "hide": true,
        "iconColor": "rgba(0, 211, 255, 1)",
        "name": "Annotations & Alerts",
        "target": {
          "limit": 100,
          "matchAny": false,
          "tags": [],
          "type": "dashboard"
        },
        "type": "dashboard"
      }
    ]
  },
  "description": "WindowsPrometheus",
  "editable": true,
  "fiscalYearStartMonth": 0,
  "gnetId": 10467,
  "graphTooltip": 1,
  "id": 28,
  "iteration": 1639901955519,
  "links": [
    {
      "icon": "bolt",
      "tags": [],
      "targetBlank": true,
      "title": "Update",
      "tooltip": "更新当前仪表板",
      "type": "link",
      "url": "https://grafana.com/grafana/dashboards/10467"
    },
    {
      "icon": "question",
      "tags": [],
      "targetBlank": true,
      "title": "GitHub",
      "tooltip": "查看更多仪表板",
      "type": "link",
      "url": "https://github.com/starsliao/Prometheus"
    },
    {
      "asDropdown": true,
      "icon": "external link",
      "tags": [],
      "targetBlank": true,
      "type": "dashboards"
    }
  ],
  "liveNow": false,
  "panels": [
    {
      "collapsed": false,
      "datasource": "Prometheus",
      "gridPos": {
        "h": 1,
        "w": 24,
        "x": 0,
        "y": 0
      },
      "id": 41,
      "panels": [],
      "title": " $show_hostname  ($instance)",
      "type": "row"
    },
    {
      "columns": [],
      "datasource": "Prometheus",
      "description": "",
      "fontSize": "80%",
      "gridPos": {
        "h": 6,
        "w": 24,
        "x": 0,
        "y": 1
      },
      "id": 45,
      "pageSize": null,
      "showHeader": true,
      "sort": {
        "col": 0,
        "desc": true
      },
      "styles": [
        {
          "$$hashKey": "object:1557",
          "alias": "product",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "product",
          "preserveFormat": false,
          "sanitize": false,
          "thresholds": [],
          "type": "string",
          "unit": "short",
          "valueMaps": []
        },
        {
          "$$hashKey": "object:1570",
          "alias": "hostname",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "link": false,
          "linkTooltip": "",
          "linkUrl": "",
          "mappingType": 1,
          "pattern": "hostname",
          "preserveFormat": false,
          "thresholds": [],
          "type": "string",
          "unit": "short"
        },
        {
          "$$hashKey": "object:1609",
          "alias": "instance",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "link": true,
          "linkTargetBlank": false,
          "linkTooltip": "${__cell_4}",
          "linkUrl": "/d/Kdh0OoSGz/?var-job=${__cell_5}&var-hostname=All&var-instance=${__cell_4}",
          "mappingType": 1,
          "pattern": "instance",
          "thresholds": [],
          "type": "string",
          "unit": "short"
        },
        {
          "$$hashKey": "object:1622",
          "alias": "CPU",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #B",
          "thresholds": [],
          "type": "string",
          "unit": "short"
        },
        {
          "$$hashKey": "object:1635",
          "alias": "Total Ram",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": null,
          "mappingType": 1,
          "pattern": "Value #C",
          "thresholds": [],
          "type": "number",
          "unit": "bytes"
        },
        {
          "$$hashKey": "object:2635",
          "alias": "UPTIME",
          "align": "auto",
          "colorMode": "cell",
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": null,
          "mappingType": 1,
          "pattern": "Value #D",
          "thresholds": [
            "259200",
            "432000"
          ],
          "type": "number",
          "unit": "s"
        },
        {
          "$$hashKey": "object:1809",
          "alias": "Disk usage rate",
          "align": "auto",
          "colorMode": "cell",
          "colors": [
            "rgba(50, 172, 45, 0.97)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(245, 54, 54, 0.9)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #E",
          "thresholds": [
            "60",
            "80"
          ],
          "type": "number",
          "unit": "percentunit"
        },
        {
          "$$hashKey": "object:1821",
          "alias": "Most used partitions",
          "align": "auto",
          "colorMode": "cell",
          "colors": [
            "rgba(50, 172, 45, 0.97)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(245, 54, 54, 0.9)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #F",
          "thresholds": [
            "60",
            "80"
          ],
          "type": "number",
          "unit": "percentunit"
        },
        {
          "$$hashKey": "object:2286",
          "alias": "Number of processes",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "link": false,
          "mappingType": 1,
          "pattern": "Value #G",
          "thresholds": [],
          "type": "string",
          "unit": "short"
        },
        {
          "$$hashKey": "object:2297",
          "alias": "Number of Service",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #H",
          "thresholds": [],
          "type": "string",
          "unit": "short"
        },
        {
          "$$hashKey": "object:3599",
          "alias": "CPU Usage",
          "align": "auto",
          "colorMode": "cell",
          "colors": [
            "rgba(50, 172, 45, 0.97)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(245, 54, 54, 0.9)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #I",
          "thresholds": [
            "50",
            "70"
          ],
          "type": "number",
          "unit": "percent"
        },
        {
          "$$hashKey": "object:3610",
          "alias": "Memory usage",
          "align": "auto",
          "colorMode": "cell",
          "colors": [
            "rgba(50, 172, 45, 0.97)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(245, 54, 54, 0.9)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #J",
          "thresholds": [
            "60",
            "80"
          ],
          "type": "number",
          "unit": "percent"
        },
        {
          "$$hashKey": "object:5929",
          "alias": "CPU Hz",
          "align": "auto",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "dateFormat": "YYYY-MM-DD HH:mm:ss",
          "decimals": 2,
          "mappingType": 1,
          "pattern": "Value #K",
          "thresholds": [],
          "type": "number",
          "unit": "rothz"
        },
        {
          "$$hashKey": "object:1311",
          "alias": "",
          "align": "right",
          "colorMode": null,
          "colors": [
            "rgba(245, 54, 54, 0.9)",
            "rgba(237, 129, 40, 0.89)",
            "rgba(50, 172, 45, 0.97)"
          ],
          "decimals": 2,
          "pattern": "/.*/",
          "thresholds": [],
          "type": "hidden",
          "unit": "short"
        }
      ],
      "targets": [
        {
          "expr": "windows_os_info{job=~\"$job\"} * on(instance) group_right(product) windows_cs_hostname",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "A"
        },
        {
          "expr": "time() - windows_system_system_up_time{job=~\"$job\"}",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "D"
        },
        {
          "expr": "windows_cs_logical_processors{job=~\"$job\"} - 0",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "B"
        },
        {
          "expr": "avg by (instance) (windows_cpu_core_frequency_mhz{job=~\"$job\"})",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "K"
        },
        {
          "expr": "100 - (avg by (instance) (irate(windows_cpu_time_total{job=~\"$job\",mode=\"idle\"}[2m])) * 100)",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "CPU使用率",
          "refId": "I"
        },
        {
          "expr": "windows_cs_physical_memory_bytes{job=~\"$job\"} - 0",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "C"
        },
        {
          "expr": "100 - 100 * windows_os_physical_memory_free_bytes{job=~\"$job\"} / windows_cs_physical_memory_bytes{job=~\"$job\"}",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "内存使用率",
          "refId": "J"
        },
        {
          "expr": "1 - (windows_logical_disk_free_bytes{job=~\"$job\",volume=~\"C:\"}/windows_logical_disk_size_bytes{job=~\"$job\",volume=~\"C:\"})",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "E"
        },
        {
          "expr": "max by (instance) (1-windows_logical_disk_free_bytes{job=~\"$job\"}/windows_logical_disk_size_bytes{job=~\"$job\"})",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "F"
        },
        {
          "expr": "windows_os_processes{job=~\"$job\"}",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "G"
        },
        {
          "expr": "sum by (instance) (windows_service_state{job=~\"$job\",state=~\"running\"})",
          "format": "table",
          "instant": true,
          "interval": "",
          "legendFormat": "",
          "refId": "H"
        }
      ],
      "timeFrom": null,
      "timeShift": null,
      "title": "$job",
      "transform": "table",
      "type": "table-old"
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "decimals": 1,
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 5,
        "x": 0,
        "y": 7
      },
      "hiddenSeries": false,
      "id": 47,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": true,
        "show": false,
        "sort": "current",
        "sortDesc": false,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "paceLength": 10,
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "100 - (avg by (instance) (irate(windows_cpu_time_total{job=~\"$job\",mode=\"idle\"}[2m])) * 100)",
          "hide": false,
          "interval": "",
          "intervalFactor": 1,
          "legendFormat": "{{instance}}",
          "refId": "B"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "CPU USAGE",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "cumulative"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:3535",
          "format": "percent",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": "0",
          "show": true
        },
        {
          "$$hashKey": "object:3536",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {
        "Free Physical memory": "semi-dark-green",
        "Free physical memory": "semi-dark-green",
        "Free virtual memory": "super-light-blue",
        "Physical memory": "dark-red",
        "Virtual memory": "dark-blue"
      },
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 1,
      "gridPos": {
        "h": 6,
        "w": 5,
        "x": 5,
        "y": 7
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 49,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": true,
        "show": false,
        "sort": "current",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 2,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [
        {
          "$$hashKey": "object:3675",
          "alias": "/.*Physical.*/",
          "linewidth": 3
        }
      ],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "100.0 - 100 * windows_os_physical_memory_free_bytes{job=~\"$job\"} / windows_cs_physical_memory_bytes{job=~\"$job\"}",
          "instant": false,
          "interval": "",
          "legendFormat": "{{instance}}",
          "refId": "A"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Memory usage",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:3688",
          "format": "percent",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:3689",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 5,
        "x": 10,
        "y": 7
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 53,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": true,
        "show": false,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "max by (instance) (irate(windows_net_bytes_sent_total{job=~\"$job\",nic!~'isatap.*|VPN.*'}[2m]))*8",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_上传",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 10
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "-max by (instance) (irate(windows_net_bytes_received_total{job=~\"$job\",nic!~'isatap.*|VPN.*'}[2m]))*8",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_下载",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 10
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Network details of the maximum traffic network card",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:4930",
          "format": "bps",
          "label": "下载　　　　上传",
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:4931",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 2,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 5,
        "x": 15,
        "y": 7
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 51,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": true,
        "show": false,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "-max by (instance) (irate(windows_logical_disk_read_bytes_total[2m]))",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_读取",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 20
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "max by (instance) (irate(windows_logical_disk_write_bytes_total[2m]))",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_写入",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Maximum disk read and write details",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:5258",
          "format": "Bps",
          "label": "读取　　　　写入",
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:5259",
          "decimals": null,
          "format": "iops",
          "label": "",
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 4,
        "x": 20,
        "y": 7
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 55,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": true,
        "show": false,
        "sort": "current",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "-max by (instance) (irate(windows_logical_disk_reads_total[2m]))",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_读取",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 20
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "max by (instance) (irate(windows_logical_disk_writes_total[2m]))",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{instance}}_写入",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "C",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Disk IO",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:5486",
          "format": "iops",
          "label": "读取　　　　写入",
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:5487",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "collapsed": false,
      "datasource": "Prometheus",
      "gridPos": {
        "h": 1,
        "w": 24,
        "x": 0,
        "y": 13
      },
      "id": 43,
      "panels": [],
      "title": "$show_hostname：$instance",
      "type": "row"
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "description": "",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "decimals": 0,
          "mappings": [
            {
              "options": {
                "match": "null",
                "result": {
                  "text": "N/A"
                }
              },
              "type": "special"
            }
          ],
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "green",
                "value": null
              },
              {
                "color": "red",
                "value": 80
              }
            ]
          },
          "unit": "ms"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 2,
        "w": 2,
        "x": 0,
        "y": 14
      },
      "id": 33,
      "interval": "",
      "links": [],
      "maxDataPoints": 100,
      "options": {
        "colorMode": "value",
        "graphMode": "none",
        "justifyMode": "auto",
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "/^windows_system_system_up_time\\{instance=\"192\\.168.10.15:9182\", job=\"Windows\\-Exporter\"\\}$/",
          "values": false
        },
        "text": {},
        "textMode": "auto"
      },
      "pluginVersion": "8.2.2",
      "repeat": "host",
      "repeatDirection": "v",
      "targets": [
        {
          "exemplar": true,
          "expr": "windows_system_system_up_time{job=~\"$job\",instance=~\"$instance\"}",
          "instant": false,
          "interval": "",
          "legendFormat": "",
          "refId": "A"
        }
      ],
      "timeFrom": null,
      "timeShift": null,
      "title": "Uptime",
      "type": "stat"
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "mappings": [
            {
              "options": {
                "": {
                  "text": ""
                }
              },
              "type": "value"
            }
          ],
          "max": 100,
          "min": 0,
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "#299c46",
                "value": null
              },
              {
                "color": "rgba(237, 129, 40, 0.89)",
                "value": 60
              },
              {
                "color": "#d44a3a",
                "value": 90
              }
            ]
          },
          "unit": "percent"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 3,
        "w": 2,
        "x": 2,
        "y": 14
      },
      "id": 19,
      "interval": null,
      "links": [],
      "maxDataPoints": 100,
      "options": {
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "",
          "values": false
        },
        "showThresholdLabels": false,
        "showThresholdMarkers": true,
        "text": {}
      },
      "pluginVersion": "8.2.2",
      "targets": [
        {
          "expr": "100 - (avg(irate(windows_cpu_time_total{job=~\"$job\",instance=~\"$instance\",mode=\"idle\"}[2m])))*100",
          "format": "time_series",
          "interval": "",
          "intervalFactor": 1,
          "legendFormat": "",
          "refId": "A"
        }
      ],
      "title": "CPU Usage Rate",
      "type": "gauge"
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "mappings": [],
          "max": 100,
          "min": 0,
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "green",
                "value": null
              },
              {
                "color": "#EAB839",
                "value": 80
              },
              {
                "color": "red",
                "value": 90
              }
            ]
          },
          "unit": "percent"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 6,
        "w": 4,
        "x": 4,
        "y": 14
      },
      "id": 23,
      "links": [],
      "options": {
        "displayMode": "lcd",
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "",
          "values": false
        },
        "showUnfilled": true,
        "text": {}
      },
      "pluginVersion": "8.2.2",
      "targets": [
        {
          "expr": "100 - (windows_logical_disk_free_bytes{job=~\"$job\",instance=~\"$instance\"} / windows_logical_disk_size_bytes{job=~\"$job\",instance=~\"$instance\"})*100",
          "instant": false,
          "interval": "",
          "legendFormat": "{{volume}}",
          "refId": "A"
        }
      ],
      "timeFrom": null,
      "timeShift": null,
      "title": "Partition Usage",
      "type": "bargauge"
    },
    {
      "aliasColors": {
        "Free Physical memory": "semi-dark-green",
        "Free physical memory": "semi-dark-green",
        "Free virtual memory": "yellow",
        "Physical memory": "dark-red",
        "Virtual memory": "dark-purple",
        "剩余物理内存": "green",
        "总物理内存": "dark-red"
      },
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "decimals": 2,
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 3,
      "gridPos": {
        "h": 6,
        "w": 8,
        "x": 8,
        "y": 14
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 14,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 0,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [
        {
          "$$hashKey": "object:225",
          "alias": "/.*物理内存.*/",
          "linewidth": 2
        }
      ],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "windows_cs_physical_memory_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "总物理内存",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 5
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "windows_os_physical_memory_free_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "剩余物理内存",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "C",
          "step": 5
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "windows_os_virtual_memory_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "Virtual memory",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 5
        },
        {
          "expr": "windows_os_virtual_memory_free_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "intervalFactor": 1,
          "legendFormat": "Free virtual memory",
          "refId": "D"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Memory details",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:197",
          "format": "bytes",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": "0",
          "show": true
        },
        {
          "$$hashKey": "object:198",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "decimals": null,
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 8,
        "x": 16,
        "y": 14
      },
      "hiddenSeries": false,
      "id": 27,
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": true,
        "max": false,
        "min": false,
        "rightSide": true,
        "show": false,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 2,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "paceLength": 10,
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [
        {
          "$$hashKey": "object:940",
          "alias": "进程数",
          "color": "#B877D9"
        }
      ],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "expr": "windows_os_processes{job=~\"$job\",instance=~\"$instance\"}",
          "instant": false,
          "interval": "",
          "legendFormat": "进程数",
          "refId": "A"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Number of processes",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:87",
          "decimals": 0,
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:88",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "description": "",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "decimals": 0,
          "mappings": [
            {
              "options": {
                "match": "null",
                "result": {
                  "text": "N/A"
                }
              },
              "type": "special"
            }
          ],
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "green",
                "value": null
              },
              {
                "color": "red",
                "value": 80
              }
            ]
          },
          "unit": "none"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 2,
        "w": 2,
        "x": 0,
        "y": 16
      },
      "id": 35,
      "interval": "",
      "links": [],
      "maxDataPoints": 100,
      "options": {
        "colorMode": "value",
        "graphMode": "none",
        "justifyMode": "auto",
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "",
          "values": false
        },
        "text": {},
        "textMode": "auto"
      },
      "pluginVersion": "8.2.2",
      "repeat": "host",
      "repeatDirection": "v",
      "targets": [
        {
          "exemplar": true,
          "expr": "windows_cs_logical_processors{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "instant": false,
          "interval": "",
          "intervalFactor": 1,
          "legendFormat": "",
          "refId": "A"
        }
      ],
      "timeFrom": null,
      "timeShift": null,
      "title": "CPU Proccesor",
      "type": "stat"
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "mappings": [
            {
              "options": {
                "match": "null",
                "result": {
                  "text": "N/A"
                }
              },
              "type": "special"
            }
          ],
          "max": 100,
          "min": 0,
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "#299c46",
                "value": null
              },
              {
                "color": "rgba(237, 129, 40, 0.89)",
                "value": 80
              },
              {
                "color": "#d44a3a",
                "value": 90
              }
            ]
          },
          "unit": "percent"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 3,
        "w": 2,
        "x": 2,
        "y": 17
      },
      "id": 21,
      "interval": null,
      "links": [],
      "maxDataPoints": 100,
      "options": {
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "/^\\{instance=\"192\\.168.10.15:9182\", job=\"Windows\\-Exporter\"\\}$/",
          "values": false
        },
        "showThresholdLabels": false,
        "showThresholdMarkers": true,
        "text": {}
      },
      "pluginVersion": "8.2.2",
      "targets": [
        {
          "expr": "100 - (windows_os_physical_memory_free_bytes{job=~\"$job\",instance=~\"$instance\"} / windows_cs_physical_memory_bytes{job=~\"$job\",instance=~\"$instance\"})*100",
          "instant": false,
          "refId": "A"
        }
      ],
      "title": "Memory usage",
      "type": "gauge"
    },
    {
      "cacheTimeout": null,
      "datasource": "Prometheus",
      "description": "",
      "fieldConfig": {
        "defaults": {
          "color": {
            "mode": "thresholds"
          },
          "decimals": 1,
          "mappings": [
            {
              "options": {
                "match": "null",
                "result": {
                  "text": "N/A"
                }
              },
              "type": "special"
            }
          ],
          "thresholds": {
            "mode": "absolute",
            "steps": [
              {
                "color": "green",
                "value": null
              },
              {
                "color": "red",
                "value": 80
              }
            ]
          },
          "unit": "bytes"
        },
        "overrides": []
      },
      "gridPos": {
        "h": 2,
        "w": 2,
        "x": 0,
        "y": 18
      },
      "id": 37,
      "interval": "",
      "links": [],
      "maxDataPoints": 100,
      "options": {
        "colorMode": "value",
        "graphMode": "none",
        "justifyMode": "auto",
        "orientation": "horizontal",
        "reduceOptions": {
          "calcs": [
            "lastNotNull"
          ],
          "fields": "",
          "values": false
        },
        "text": {},
        "textMode": "auto"
      },
      "pluginVersion": "8.2.2",
      "repeat": "host",
      "repeatDirection": "v",
      "targets": [
        {
          "exemplar": true,
          "expr": "windows_cs_physical_memory_bytes{instance=\"192.168.10.15:9182\", job=\"Windows-Exporter\"}",
          "format": "time_series",
          "instant": false,
          "interval": "",
          "intervalFactor": 1,
          "legendFormat": "",
          "refId": "A"
        }
      ],
      "timeFrom": null,
      "timeShift": null,
      "title": "Total Ram",
      "type": "stat"
    },
    {
      "aliasColors": {
        "Received mysqld-exporter:9104": "#0A50A1",
        "stopped": "#2F575E"
      },
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "unit": "none"
        },
        "overrides": []
      },
      "fill": 10,
      "fillGradient": 0,
      "gridPos": {
        "h": 7,
        "w": 8,
        "x": 0,
        "y": 20
      },
      "hiddenSeries": false,
      "id": 57,
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": false,
        "max": false,
        "min": false,
        "rightSide": true,
        "show": true,
        "total": false,
        "values": false
      },
      "lines": true,
      "linewidth": 0,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": true,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "sum(windows_service_status{instance=~\"$server\"}) by (status)",
          "functions": [],
          "group": {
            "filter": ""
          },
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{status}}",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 5
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "windows_service_status",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:284",
          "format": "none",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:285",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {
        "Received mysqld-exporter:9104": "#0A50A1",
        "stopped": "#2F575E"
      },
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 10,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 8,
        "x": 8,
        "y": 20
      },
      "hiddenSeries": false,
      "id": 7,
      "legend": {
        "alignAsTable": true,
        "avg": false,
        "current": true,
        "max": false,
        "min": false,
        "rightSide": true,
        "show": true,
        "sort": "current",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 0,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": true,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "sum(windows_service_state{job=~\"$job\",instance=~\"$instance\"}) by (state)",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{state}}",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 5
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "service status",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:570",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:571",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 0,
      "fillGradient": 0,
      "gridPos": {
        "h": 8,
        "w": 8,
        "x": 16,
        "y": 20
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 15,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 2,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [
        {
          "$$hashKey": "object:7159",
          "alias": "/总空间.*/",
          "color": "#F2495C"
        }
      ],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "windows_logical_disk_free_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "Drive{{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 20
        },
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "windows_logical_disk_size_bytes{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "Drive {{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Free disk space",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:312",
          "format": "decbytes",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": "0",
          "show": true
        },
        {
          "$$hashKey": "object:313",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 2,
      "fillGradient": 0,
      "gridPos": {
        "h": 8,
        "w": 8,
        "x": 8,
        "y": 26
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 8,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "sort": null,
        "sortDesc": null,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_logical_disk_read_bytes_total{job=~\"$job\",instance=~\"$instance\"}[5m])\r",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "read {{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 20
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_logical_disk_write_bytes_total{job=~\"$job\",instance=~\"$instance\"}[5m])\r",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "write {{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Disk read and write",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:761",
          "format": "Bps",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:762",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "decimals": 1,
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 7,
        "w": 8,
        "x": 0,
        "y": 27
      },
      "hiddenSeries": false,
      "id": 25,
      "legend": {
        "alignAsTable": false,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "sort": "current",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "paceLength": 10,
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": true,
      "steppedLine": false,
      "targets": [
        {
          "exemplar": true,
          "expr": "100 - avg(irate(windows_cpu_time_total{job=~\"$job\",instance=~\"$instance\",mode=\"idle\"}[5m]))*100",
          "hide": false,
          "interval": "",
          "legendFormat": "CPU Usage",
          "refId": "A"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "CPU Usage rate",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:366",
          "format": "percent",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:367",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 8,
        "w": 8,
        "x": 16,
        "y": 28
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 9,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_logical_disk_reads_total{job=~\"$job\",instance=~\"$instance\"}[5m])",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "read {{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 20
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_logical_disk_writes_total{job=~\"$job\",instance=~\"$instance\"}[5m])",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "write {{volume}}",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "C",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Disk IO",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:815",
          "format": "iops",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:816",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 7,
        "w": 8,
        "x": 0,
        "y": 34
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 13,
      "legend": {
        "alignAsTable": false,
        "avg": false,
        "current": true,
        "max": true,
        "min": false,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_system_exception_dispatches_total{job=~\"$job\",instance=~\"$instance\"}[5m])",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "exceptions",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "System exception dispatches",
      "tooltip": {
        "shared": false,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:466",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:467",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 7,
        "w": 8,
        "x": 8,
        "y": 34
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 12,
      "legend": {
        "alignAsTable": false,
        "avg": false,
        "current": true,
        "max": false,
        "min": false,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "expr": "windows_system_threads{job=~\"$job\",instance=~\"$instance\"}",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "system_threads",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 20
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "system_threads",
      "tooltip": {
        "shared": false,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:414",
          "format": "none",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:415",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 11,
        "w": 8,
        "x": 16,
        "y": 36
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 11,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": true,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": true,
        "sort": "max",
        "sortDesc": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "irate(windows_net_bytes_sent_total{job=~\"$job\",instance=~\"$instance\",nic!~'isatap.*|VPN.*'}[5m])*8>0\r",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{nic}}-Sent",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 10
        },
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "irate(windows_net_bytes_received_total{job=~\"$job\",instance=~\"$instance\",nic!~'isatap.*|VPN.*'}[5m])*8\n",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "{{nic}}-Received",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 10
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Network details",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:137",
          "format": "bps",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:138",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": false
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": true,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "decimals": 2,
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 6,
        "x": 0,
        "y": 41
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 29,
      "legend": {
        "alignAsTable": true,
        "avg": true,
        "current": false,
        "max": true,
        "min": true,
        "rightSide": false,
        "show": false,
        "total": false,
        "values": true
      },
      "lines": false,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null",
      "options": {
        "alertThreshold": true
      },
      "paceLength": 10,
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": true,
      "steppedLine": false,
      "targets": [
        {
          "expr": "(irate(windows_net_bytes_total{job=~\"$job\",instance=~\"$instance\",nic!~'isatap.*|VPN.*'}[5m]) * 8 / windows_net_current_bandwidth{job=~\"$job\",instance=~\"$instance\",nic!~'isatap.*|VPN.*'}) * 100",
          "legendFormat": "{{nic}}",
          "refId": "A"
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Network usage",
      "tooltip": {
        "shared": true,
        "sort": 0,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:915",
          "format": "percent",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:916",
          "format": "bytes",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    },
    {
      "aliasColors": {},
      "bars": false,
      "dashLength": 10,
      "dashes": false,
      "datasource": "Prometheus",
      "fieldConfig": {
        "defaults": {
          "links": []
        },
        "overrides": []
      },
      "fill": 1,
      "fillGradient": 0,
      "gridPos": {
        "h": 6,
        "w": 10,
        "x": 6,
        "y": 41
      },
      "hiddenSeries": false,
      "hideTimeOverride": false,
      "id": 10,
      "legend": {
        "alignAsTable": false,
        "avg": false,
        "current": true,
        "max": false,
        "min": false,
        "rightSide": false,
        "show": true,
        "total": false,
        "values": true
      },
      "lines": true,
      "linewidth": 1,
      "links": [],
      "nullPointMode": "null as zero",
      "options": {
        "alertThreshold": true
      },
      "percentage": false,
      "pluginVersion": "8.2.2",
      "pointradius": 5,
      "points": false,
      "renderer": "flot",
      "seriesOverrides": [],
      "spaceLength": 10,
      "stack": false,
      "steppedLine": false,
      "targets": [
        {
          "application": {
            "filter": ""
          },
          "exemplar": true,
          "expr": "irate(windows_net_packets_outbound_discarded{job=~\"$job\",instance=~\"$instance\", nic!~'isatap.*|VPN.*'}[5m]) + irate(windows_net_packets_outbound_errors{job=~\"$job\",instance=~\"$instance\"}[5m])",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "outbound",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "B",
          "step": 15
        },
        {
          "application": {
            "filter": ""
          },
          "expr": "irate(windows_net_packets_received_discarded{job=~\"$job\",instance=~\"$instance\", nic!~'isatap.*|VPN.*'}[5m]) + irate(windows_net_packets_received_errors{job=~\"$job\",instance=~\"$instance\"}[5m])",
          "format": "time_series",
          "functions": [],
          "group": {
            "filter": ""
          },
          "hide": false,
          "host": {
            "filter": ""
          },
          "interval": "",
          "intervalFactor": 1,
          "item": {
            "filter": ""
          },
          "legendFormat": "received",
          "metric": "mysql_global_status_questions",
          "mode": 0,
          "options": {
            "showDisabledItems": false
          },
          "refId": "A",
          "step": 15
        }
      ],
      "thresholds": [],
      "timeFrom": null,
      "timeRegions": [],
      "timeShift": null,
      "title": "Network discarded/error packets",
      "tooltip": {
        "shared": true,
        "sort": 2,
        "value_type": "individual"
      },
      "type": "graph",
      "xaxis": {
        "buckets": null,
        "mode": "time",
        "name": null,
        "show": true,
        "values": []
      },
      "yaxes": [
        {
          "$$hashKey": "object:518",
          "format": "pps",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        },
        {
          "$$hashKey": "object:519",
          "format": "short",
          "label": null,
          "logBase": 1,
          "max": null,
          "min": null,
          "show": true
        }
      ],
      "yaxis": {
        "align": false,
        "alignLevel": null
      }
    }
  ],
  "refresh": false,
  "schemaVersion": 31,
  "style": "dark",
  "tags": [],
  "templating": {
    "list": [
      {
        "allValue": null,
        "current": {
          "selected": false,
          "text": "Windows-Exporter",
          "value": "Windows-Exporter"
        },
        "datasource": "Prometheus",
        "definition": "label_values(windows_cs_hostname, job)",
        "description": null,
        "error": null,
        "hide": 0,
        "includeAll": false,
        "label": "JOB",
        "multi": false,
        "name": "job",
        "options": [],
        "query": {
          "query": "label_values(windows_cs_hostname, job)",
          "refId": "Prometheus-job-Variable-Query"
        },
        "refresh": 1,
        "regex": "",
        "skipUrlSync": false,
        "sort": 1,
        "tagValuesQuery": "",
        "tagsQuery": "",
        "type": "query",
        "useTags": false
      },
      {
        "allValue": null,
        "current": {
          "selected": false,
          "text": "All",
          "value": "$__all"
        },
        "datasource": "Prometheus",
        "definition": "label_values(windows_cs_hostname{job=~\"$job\"}, hostname)",
        "description": null,
        "error": null,
        "hide": 0,
        "includeAll": true,
        "label": "主机名",
        "multi": false,
        "name": "hostname",
        "options": [],
        "query": {
          "query": "label_values(windows_cs_hostname{job=~\"$job\"}, hostname)",
          "refId": "Prometheus-hostname-Variable-Query"
        },
        "refresh": 1,
        "regex": "",
        "skipUrlSync": false,
        "sort": 5,
        "tagValuesQuery": "",
        "tagsQuery": "",
        "type": "query",
        "useTags": false
      },
      {
        "allValue": null,
        "current": {
          "selected": false,
          "text": "192.168.10.15:9182",
          "value": "192.168.10.15:9182"
        },
        "datasource": "Prometheus",
        "definition": "label_values(windows_cs_hostname{job=~\"$job\",hostname=~\"$hostname\"}, instance)",
        "description": null,
        "error": null,
        "hide": 0,
        "includeAll": false,
        "label": "instance",
        "multi": false,
        "name": "instance",
        "options": [],
        "query": {
          "query": "label_values(windows_cs_hostname{job=~\"$job\",hostname=~\"$hostname\"}, instance)",
          "refId": "Prometheus-instance-Variable-Query"
        },
        "refresh": 1,
        "regex": "",
        "skipUrlSync": false,
        "sort": 5,
        "tagValuesQuery": "",
        "tagsQuery": "",
        "type": "query",
        "useTags": false
      },
      {
        "allValue": null,
        "current": {
          "selected": false,
          "text": "server4",
          "value": "server4"
        },
        "datasource": "Prometheus",
        "definition": "label_values(windows_cs_hostname{job=~\"$job\",instance=~\"$instance\"}, hostname)",
        "description": null,
        "error": null,
        "hide": 2,
        "includeAll": false,
        "label": "展示使用的主机名",
        "multi": false,
        "name": "show_hostname",
        "options": [],
        "query": {
          "query": "label_values(windows_cs_hostname{job=~\"$job\",instance=~\"$instance\"}, hostname)",
          "refId": "Prometheus-show_hostname-Variable-Query"
        },
        "refresh": 1,
        "regex": "",
        "skipUrlSync": false,
        "sort": 0,
        "tagValuesQuery": "",
        "tagsQuery": "",
        "type": "query",
        "useTags": false
      },
      {
        "allValue": null,
        "current": {
          "selected": false,
          "text": "192.168.10.15:9182",
          "value": "192.168.10.15:9182"
        },
        "datasource": null,
        "definition": "label_values(windows_system_system_up_time, instance)",
        "description": null,
        "error": null,
        "hide": 0,
        "includeAll": false,
        "label": "server",
        "multi": false,
        "name": "server",
        "options": [],
        "query": {
          "query": "label_values(windows_system_system_up_time, instance)",
          "refId": "StandardVariableQuery"
        },
        "refresh": 1,
        "regex": "",
        "skipUrlSync": false,
        "sort": 0,
        "type": "query"
      }
    ]
  },
  "time": {
    "from": "now-3h",
    "to": "now"
  },
  "timepicker": {
    "refresh_intervals": [
      "10s",
      "30s",
      "1m",
      "5m",
      "15m",
      "30m",
      "1h",
      "2h",
      "1d"
    ],
    "time_options": [
      "5m",
      "15m",
      "1h",
      "6h",
      "12h",
      "24h",
      "2d",
      "7d",
      "30d"
    ]
  },
  "timezone": "",
  "title": "windows_exporter for Prometheus Dashboard CN v20201012 Copy",
  "uid": "G6DBBFT7k",
  "version": 1
}

```

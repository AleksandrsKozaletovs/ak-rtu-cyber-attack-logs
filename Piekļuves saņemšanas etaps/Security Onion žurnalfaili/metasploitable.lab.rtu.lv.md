**Atklata uzbrukuma žurnalfails JSON formatā**
```json
{
  "_index": ".ds-logs-suricata.alerts-so-2025.05.21-000011",
  "_id": "MahB-ZYBy3bp7Al2n_zn",
  "_version": 1,
  "_source": {
    "metadata": {
      "pipeline": "suricata.common",
      "input": {
        "beats": {
          "host": {
            "ip": "192.168.1.100"
          }
        }
      },
      "raw_index": "logs-suricata-so",
      "stream_id": "logfile-log.logs-d08eaf9d-db60-4107-8711-186f5eb33d1f",
      "beat": "filebeat",
      "type": "_doc",
      "version": "8.17.3",
      "input_id": "logfile-logs-d08eaf9d-db60-4107-8711-186f5eb33d1f"
    },
    "log": {
      "file": {
        "path": "/nsm/suricata/eve-2025-05-22-18:19.json"
      },
      "offset": 6228,
      "id": {
        "uid": "788739358610233"
      }
    },
    "elastic_agent": {
      "id": "c8bcdb8e-0b07-4cd8-854b-ce380c3559ed",
      "version": "8.17.3",
      "snapshot": false
    },
    "destination": {
      "port": 39391,
      "ip": "192.168.1.175"
    },
    "rule": {
      "severity": 2,
      "reference": "https://community.emergingthreats.net",
      "rev": 7,
      "metadata": {
        "updated_at": [
          "2019_07_26"
        ],
        "confidence": [
          "Medium"
        ],
        "created_at": [
          "2010_09_23"
        ],
        "signature_severity": [
          "Informational"
        ]
      },
      "gid": 1,
      "name": "GPL ATTACK_RESPONSE id check returned root",
      "ruleset": "Snort GPL",
      "action": "allowed",
      "rule": "alert ip any any -> any any (msg:\"GPL ATTACK_RESPONSE id check returned root\"; content:\"uid=0|28|root|29|\"; classtype:bad-unknown; sid:2100498; rev:7; metadata:created_at 2010_09_23, confidence Medium, signature_severity Informational, updated_at 2019_07_26;)",
      "category": "Potentially Bad Traffic",
      "uuid": "2100498"
    },
    "source": {
      "port": 6200,
      "ip": "192.168.1.11"
    },
    "message": "{\"timestamp\":\"2025-05-22T18:28:56.590317+0000\",\"flow_id\":788739358610233,\"in_iface\":\"bond0\",\"event_type\":\"alert\",\"src_ip\":\"192.168.1.11\",\"src_port\":6200,\"dest_ip\":\"192.168.1.175\",\"dest_port\":39391,\"proto\":\"TCP\",\"pkt_src\":\"stream (flow timeout)\",\"community_id\":\"1:4VUkJupYhA6RP+xhGL5c62H+GNQ=\",\"alert\":{\"action\":\"allowed\",\"gid\":1,\"signature_id\":2100498,\"rev\":7,\"signature\":\"GPL ATTACK_RESPONSE id check returned root\",\"category\":\"Potentially Bad Traffic\",\"severity\":2,\"metadata\":{\"confidence\":[\"Medium\"],\"created_at\":[\"2010_09_23\"],\"signature_severity\":[\"Informational\"],\"updated_at\":[\"2019_07_26\"]},\"rule\":\"alert ip any any -> any any (msg:\\\"GPL ATTACK_RESPONSE id check returned root\\\"; content:\\\"uid=0|28|root|29|\\\"; classtype:bad-unknown; sid:2100498; rev:7; metadata:created_at 2010_09_23, confidence Medium, signature_severity Informational, updated_at 2019_07_26;)\"},\"app_proto\":\"failed\",\"direction\":\"to_client\",\"payload_printable\":\"uid=0(root) gid=0(root)\\nrAkAV0vNl0yJBkDK\\nMRKlA1MvSnX3u6HeOiETZdR\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\nsh: line 7: .: command not found\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\n/\\nftp\\nmsfadmin\\nservice\\nuser\\nftp\\nmsfadmin\\nservice\\nuser\\nsh: line 13: .: command not found\\n\",\"stream\":1,\"packet\":\"RQAAKAAAAABABvbFwKgBC8CoAa8YOJnfGGb8fgAAAABQAAoAWt0AAA==\",\"packet_info\":{\"linktype\":1},\"capture_file\":\"/nsm/suripcap/1/so-pcap.1747934624\"}",
    "tags": [
      "alert",
      "alert"
    ],
    "network": {
      "community_id": "1:4VUkJupYhA6RP+xhGL5c62H+GNQ=",
      "data": {
        "decoded": "uid=0(root) gid=0(root)\nrAkAV0vNl0yJBkDK\nMRKlA1MvSnX3u6HeOiETZdR\nbin\nboot\ncdrom\ncore\ndev\netc\nhome\ninitrd\ninitrd.img\nlib\nlost+found\nmedia\nmnt\nnohup.out\nopt\nproc\nroot\nsbin\nsrv\nsys\ntmp\nusr\nvar\nvmlinuz\nsh: line 7: .: command not found\nbin\nboot\ncdrom\ncore\ndev\netc\nhome\ninitrd\ninitrd.img\nlib\nlost+found\nmedia\nmnt\nnohup.out\nopt\nproc\nroot\nsbin\nsrv\nsys\ntmp\nusr\nvar\nvmlinuz\n/\nftp\nmsfadmin\nservice\nuser\nftp\nmsfadmin\nservice\nuser\nsh: line 13: .: command not found\n"
      },
      "transport": "TCP",
      "packet_source": "stream (flow timeout)"
    },
    "input": {
      "type": "log"
    },
    "observer": {
      "ingress": {
        "interface": {
          "name": "bond0"
        }
      },
      "name": "securityonion-rtulab"
    },
    "@timestamp": "2025-05-22T18:28:56.590Z",
    "ecs": {
      "version": "8.0.0"
    },
    "data_stream": {
      "namespace": "so",
      "type": "logs",
      "dataset": "suricata"
    },
    "@version": "1",
    "event": {
      "severity": 2,
      "ingested": "2025-05-22T18:29:01.509Z",
      "module": "suricata",
      "category": "network",
      "dataset": "suricata.alert",
      "severity_label": "medium"
    }
  },
  "fields": {
    "log.id.uid": [
      "788739358610233"
    ],
    "elastic_agent.version": [
      "8.17.3"
    ],
    "event.category": [
      "network"
    ],
    "event.category.keyword": [
      "network"
    ],
    "rule.reference": [
      "https://community.emergingthreats.net"
    ],
    "event.dataset.keyword": [
      "suricata.alert"
    ],
    "observer.ingress.interface.name": [
      "bond0"
    ],
    "rule.metadata.updated_at": [
      "2019_07_26"
    ],
    "ecs.version.keyword": [
      "8.0.0"
    ],
    "metadata.stream_id": [
      "logfile-log.logs-d08eaf9d-db60-4107-8711-186f5eb33d1f"
    ],
    "rule.ruleset": [
      "Snort GPL"
    ],
    "source.ip": [
      "192.168.1.11"
    ],
    "metadata.raw_index": [
      "logs-suricata-so"
    ],
    "network.community_id": [
      "1:4VUkJupYhA6RP+xhGL5c62H+GNQ="
    ],
    "network.data.decoded": [
      "uid=0(root) gid=0(root)\nrAkAV0vNl0yJBkDK\nMRKlA1MvSnX3u6HeOiETZdR\nbin\nboot\ncdrom\ncore\ndev\netc\nhome\ninitrd\ninitrd.img\nlib\nlost+found\nmedia\nmnt\nnohup.out\nopt\nproc\nroot\nsbin\nsrv\nsys\ntmp\nusr\nvar\nvmlinuz\nsh: line 7: .: command not found\nbin\nboot\ncdrom\ncore\ndev\netc\nhome\ninitrd\ninitrd.img\nlib\nlost+found\nmedia\nmnt\nnohup.out\nopt\nproc\nroot\nsbin\nsrv\nsys\ntmp\nusr\nvar\nvmlinuz\n/\nftp\nmsfadmin\nservice\nuser\nftp\nmsfadmin\nservice\nuser\nsh: line 13: .: command not found\n"
    ],
    "rule.gid": [
      1
    ],
    "rule.name.keyword": [
      "GPL ATTACK_RESPONSE id check returned root"
    ],
    "event.severity": [
      2
    ],
    "rule.metadata.created_at": [
      "2010_09_23"
    ],
    "rule.name": [
      "GPL ATTACK_RESPONSE id check returned root"
    ],
    "source.port.keyword": [
      "6200"
    ],
    "metadata.input.beats.host.ip": [
      "192.168.1.100"
    ],
    "metadata.input.beats.host.ip.keyword": [
      "192.168.1.100"
    ],
    "input.type": [
      "log"
    ],
    "log.offset": [
      6228
    ],
    "metadata.input_id": [
      "logfile-logs-d08eaf9d-db60-4107-8711-186f5eb33d1f"
    ],
    "data_stream.type": [
      "logs"
    ],
    "tags": [
      "alert",
      "alert"
    ],
    "destination.ip.keyword": [
      "192.168.1.175"
    ],
    "source.port": [
      6200
    ],
    "ecs.version": [
      "8.0.0"
    ],
    "rule.rule": [
      "alert ip any any -> any any (msg:\"GPL ATTACK_RESPONSE id check returned root\"; content:\"uid=0|28|root|29|\"; classtype:bad-unknown; sid:2100498; rev:7; metadata:created_at 2010_09_23, confidence Medium, signature_severity Informational, updated_at 2019_07_26;)"
    ],
    "message.keyword": [
      "{\"timestamp\":\"2025-05-22T18:28:56.590317+0000\",\"flow_id\":788739358610233,\"in_iface\":\"bond0\",\"event_type\":\"alert\",\"src_ip\":\"192.168.1.11\",\"src_port\":6200,\"dest_ip\":\"192.168.1.175\",\"dest_port\":39391,\"proto\":\"TCP\",\"pkt_src\":\"stream (flow timeout)\",\"community_id\":\"1:4VUkJupYhA6RP+xhGL5c62H+GNQ=\",\"alert\":{\"action\":\"allowed\",\"gid\":1,\"signature_id\":2100498,\"rev\":7,\"signature\":\"GPL ATTACK_RESPONSE id check returned root\",\"category\":\"Potentially Bad Traffic\",\"severity\":2,\"metadata\":{\"confidence\":[\"Medium\"],\"created_at\":[\"2010_09_23\"],\"signature_severity\":[\"Informational\"],\"updated_at\":[\"2019_07_26\"]},\"rule\":\"alert ip any any -> any any (msg:\\\"GPL ATTACK_RESPONSE id check returned root\\\"; content:\\\"uid=0|28|root|29|\\\"; classtype:bad-unknown; sid:2100498; rev:7; metadata:created_at 2010_09_23, confidence Medium, signature_severity Informational, updated_at 2019_07_26;)\"},\"app_proto\":\"failed\",\"direction\":\"to_client\",\"payload_printable\":\"uid=0(root) gid=0(root)\\nrAkAV0vNl0yJBkDK\\nMRKlA1MvSnX3u6HeOiETZdR\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\nsh: line 7: .: command not found\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\n/\\nftp\\nmsfadmin\\nservice\\nuser\\nftp\\nmsfadmin\\nservice\\nuser\\nsh: line 13: .: command not found\\n\",\"stream\":1,\"packet\":\"RQAAKAAAAABABvbFwKgBC8CoAa8YOJnfGGb8fgAAAABQAAoAWt0AAA==\",\"packet_info\":{\"linktype\":1},\"capture_file\":\"/nsm/suripcap/1/so-pcap.1747934624\"}"
    ],
    "event.module.keyword": [
      "suricata"
    ],
    "event.severity_label": [
      "medium"
    ],
    "source.ip.keyword": [
      "192.168.1.11"
    ],
    "rule.metadata.signature_severity": [
      "Informational"
    ],
    "rule.rev": [
      7
    ],
    "rule.action": [
      "allowed"
    ],
    "destination.port": [
      39391
    ],
    "observer.name": [
      "securityonion-rtulab"
    ],
    "rule.metadata.confidence": [
      "Medium"
    ],
    "rule.severity": [
      2
    ],
    "tags.keyword": [
      "alert",
      "alert"
    ],
    "rule.category.keyword": [
      "Potentially Bad Traffic"
    ],
    "observer.name.keyword": [
      "securityonion-rtulab"
    ],
    "event.module": [
      "suricata"
    ],
    "event.severity_label.keyword": [
      "medium"
    ],
    "@version": [
      "1"
    ],
    "event.ingested.keyword": [
      "2025-05-22T18:29:01.509Z"
    ],
    "elastic_agent.snapshot": [
      false
    ],
    "metadata.type": [
      "_doc"
    ],
    "network.packet_source": [
      "stream (flow timeout)"
    ],
    "destination.port.keyword": [
      "39391"
    ],
    "metadata.beat": [
      "filebeat"
    ],
    "elastic_agent.id": [
      "c8bcdb8e-0b07-4cd8-854b-ce380c3559ed"
    ],
    "data_stream.namespace": [
      "so"
    ],
    "metadata.pipeline": [
      "suricata.common"
    ],
    "metadata.version": [
      "8.17.3"
    ],
    "network.transport.keyword": [
      "TCP"
    ],
    "message": [
      "{\"timestamp\":\"2025-05-22T18:28:56.590317+0000\",\"flow_id\":788739358610233,\"in_iface\":\"bond0\",\"event_type\":\"alert\",\"src_ip\":\"192.168.1.11\",\"src_port\":6200,\"dest_ip\":\"192.168.1.175\",\"dest_port\":39391,\"proto\":\"TCP\",\"pkt_src\":\"stream (flow timeout)\",\"community_id\":\"1:4VUkJupYhA6RP+xhGL5c62H+GNQ=\",\"alert\":{\"action\":\"allowed\",\"gid\":1,\"signature_id\":2100498,\"rev\":7,\"signature\":\"GPL ATTACK_RESPONSE id check returned root\",\"category\":\"Potentially Bad Traffic\",\"severity\":2,\"metadata\":{\"confidence\":[\"Medium\"],\"created_at\":[\"2010_09_23\"],\"signature_severity\":[\"Informational\"],\"updated_at\":[\"2019_07_26\"]},\"rule\":\"alert ip any any -> any any (msg:\\\"GPL ATTACK_RESPONSE id check returned root\\\"; content:\\\"uid=0|28|root|29|\\\"; classtype:bad-unknown; sid:2100498; rev:7; metadata:created_at 2010_09_23, confidence Medium, signature_severity Informational, updated_at 2019_07_26;)\"},\"app_proto\":\"failed\",\"direction\":\"to_client\",\"payload_printable\":\"uid=0(root) gid=0(root)\\nrAkAV0vNl0yJBkDK\\nMRKlA1MvSnX3u6HeOiETZdR\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\nsh: line 7: .: command not found\\nbin\\nboot\\ncdrom\\ncore\\ndev\\netc\\nhome\\ninitrd\\ninitrd.img\\nlib\\nlost+found\\nmedia\\nmnt\\nnohup.out\\nopt\\nproc\\nroot\\nsbin\\nsrv\\nsys\\ntmp\\nusr\\nvar\\nvmlinuz\\n/\\nftp\\nmsfadmin\\nservice\\nuser\\nftp\\nmsfadmin\\nservice\\nuser\\nsh: line 13: .: command not found\\n\",\"stream\":1,\"packet\":\"RQAAKAAAAABABvbFwKgBC8CoAa8YOJnfGGb8fgAAAABQAAoAWt0AAA==\",\"packet_info\":{\"linktype\":1},\"capture_file\":\"/nsm/suripcap/1/so-pcap.1747934624\"}"
    ],
    "destination.ip": [
      "192.168.1.175"
    ],
    "network.transport": [
      "TCP"
    ],
    "rule.uuid": [
      "2100498"
    ],
    "event.ingested": [
      "2025-05-22T18:29:01.509Z"
    ],
    "@timestamp": [
      "2025-05-22T18:28:56.590Z"
    ],
    "data_stream.dataset": [
      "suricata"
    ],
    "log.file.path": [
      "/nsm/suricata/eve-2025-05-22-18:19.json"
    ],
    "rule.category": [
      "Potentially Bad Traffic"
    ],
    "event.dataset": [
      "suricata.alert"
    ]
  }
}
```

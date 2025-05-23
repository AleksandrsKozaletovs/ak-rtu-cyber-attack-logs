**Security Onion žurnalfaila saturs**
```json
{
  "@timestamp": "2025-05-23T18:12:35.925Z",
  "@version": "1",
  "data_stream.dataset": "suricata",
  "data_stream.namespace": "so",
  "data_stream.type": "logs",
  "destination.ip": "146.75.118.132",
  "destination.port": 80,
  "ecs.version": "8.0.0",
  "elastic_agent.id": "c8bcdb8e-0b07-4cd8-854b-ce380c3559ed",
  "elastic_agent.snapshot": false,
  "elastic_agent.version": "8.17.3",
  "event.category": "network",
  "event.dataset": "suricata.alert",
  "event.ingested": "2025-05-23T18:12:37.895Z",
  "event.module": "suricata",
  "event.severity": 1,
  "event.severity_label": "low",
  "input.type": "log",
  "log.file.path": "/nsm/suricata/eve-2025-05-23-17:24.json",
  "log.id.uid": "973189783714172",
  "log.offset": 123353,
  "message": "{\"timestamp\":\"2025-05-23T18:12:35.925083+0000\",\"flow_id\":973189783714172,\"in_iface\":\"bond0\",\"event_type\":\"alert\",\"src_ip\":\"192.168.1.12\",\"src_port\":41934,\"dest_ip\":\"146.75.118.132\",\"dest_port\":80,\"proto\":\"TCP\",\"pkt_src\":\"wire/pcap\",\"community_id\":\"1:TRTuwGXWNyOEDubnaMV4mc8Ysrc=\",\"tx_id\":3,\"alert\":{\"action\":\"allowed\",\"gid\":1,\"signature_id\":2013504,\"rev\":6,\"signature\":\"ET INFO GNU/Linux APT User-Agent Outbound likely related to package management\",\"category\":\"Not Suspicious Traffic\",\"severity\":3,\"metadata\":{\"confidence\":[\"High\"],\"created_at\":[\"2011_08_31\"],\"signature_severity\":[\"Informational\"],\"updated_at\":[\"2020_04_22\"]},\"rule\":\"alert http $HOME_NET any -> $EXTERNAL_NET any (msg:\\\"ET INFO GNU/Linux APT User-Agent Outbound likely related to package management\\\"; flow:established,to_server; http.user_agent; content:\\\"APT-HTTP|2F|\\\"; reference:url,help.ubuntu.com/community/AptGet/Howto; classtype:not-suspicious; sid:2013504; rev:6; metadata:created_at 2011_08_31, confidence High, signature_severity Informational, updated_at 2020_04_22;)\"},\"app_proto\":\"http\",\"direction\":\"to_server\",\"payload_printable\":\"GET /debian/dists/jessie/InRelease HTTP/1.1\\r\\nHost: deb.debian.org\\r\\nCache-Control: max-age=0\\r\\nAccept: text/*\\r\\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\\r\\n\\r\\nGET /debian/dists/jessie-updates/InRelease HTTP/1.1\\r\\nHost: deb.debian.org\\r\\nCache-Control: max-age=0\\r\\nAccept: text/*\\r\\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\\r\\n\\r\\nGET /debian/dists/jessie/Release.gpg HTTP/1.1\\r\\nHost: deb.debian.org\\r\\nCache-Control: max-age=0\\r\\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\\r\\n\\r\\nGET /debian/dists/jessie-updates/Release.gpg HTTP/1.1\\r\\nHost: deb.debian.org\\r\\nCache-Control: max-age=0\\r\\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\\r\\n\\r\\n\",\"stream\":1,\"packet\":\"JC/QFleg1v3ReX76CABFAADOtNNAAEAGutLAqAEMkkt2hKPOAFDSI7+Ic8sNmoAYAd7cogAAAQEICgtziJj9T5EnR0VUIC9kZWJpYW4vZGlzdHMvamVzc2llL1JlbGVhc2UgSFRUUC8xLjENCkhvc3Q6IGRlYi5kZWJpYW4ub3JnDQpDYWNoZS1Db250cm9sOiBtYXgtYWdlPTANCkFjY2VwdDogdGV4dC8qDQpVc2VyLUFnZW50OiBEZWJpYW4gQVBULUhUVFAvMS4zICgxLjAuOS44LjQpDQoNCg==\",\"packet_info\":{\"linktype\":1},\"capture_file\":\"/nsm/suripcap/1/so-pcap.1748013414\"}",
  "metadata.beat": "filebeat",
  "metadata.input.beats.host.ip": "172.17.1.1",
  "metadata.input_id": "logfile-logs-d08eaf9d-db60-4107-8711-186f5eb33d1f",
  "metadata.pipeline": "suricata.common",
  "metadata.raw_index": "logs-suricata-so",
  "metadata.stream_id": "logfile-log.logs-d08eaf9d-db60-4107-8711-186f5eb33d1f",
  "metadata.type": "_doc",
  "metadata.version": "8.17.3",
  "network.community_id": "1:TRTuwGXWNyOEDubnaMV4mc8Ysrc=",
  "network.data.decoded": "GET /debian/dists/jessie/InRelease HTTP/1.1\r\nHost: deb.debian.org\r\nCache-Control: max-age=0\r\nAccept: text/*\r\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\r\n\r\nGET /debian/dists/jessie-updates/InRelease HTTP/1.1\r\nHost: deb.debian.org\r\nCache-Control: max-age=0\r\nAccept: text/*\r\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\r\n\r\nGET /debian/dists/jessie/Release.gpg HTTP/1.1\r\nHost: deb.debian.org\r\nCache-Control: max-age=0\r\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\r\n\r\nGET /debian/dists/jessie-updates/Release.gpg HTTP/1.1\r\nHost: deb.debian.org\r\nCache-Control: max-age=0\r\nUser-Agent: Debian APT-HTTP/1.3 (1.0.9.8.4)\r\n\r\n",
  "network.packet_source": "wire/pcap",
  "network.transport": "TCP",
  "observer.ingress.interface.name": "bond0",
  "observer.name": "securityonion-rtulab",
  "rule.action": "allowed",
  "rule.category": "Not Suspicious Traffic",
  "rule.gid": 1,
  "rule.metadata.confidence": [
    "High"
  ],
  "rule.metadata.created_at": [
    "2011_08_31"
  ],
  "rule.metadata.signature_severity": [
    "Informational"
  ],
  "rule.metadata.updated_at": [
    "2020_04_22"
  ],
  "rule.name": "ET INFO GNU/Linux APT User-Agent Outbound likely related to package management",
  "rule.reference": "https://community.emergingthreats.net",
  "rule.rev": 6,
  "rule.rule": "alert http $HOME_NET any -> $EXTERNAL_NET any (msg:\"ET INFO GNU/Linux APT User-Agent Outbound likely related to package management\"; flow:established,to_server; http.user_agent; content:\"APT-HTTP|2F|\"; reference:url,help.ubuntu.com/community/AptGet/Howto; classtype:not-suspicious; sid:2013504; rev:6; metadata:created_at 2011_08_31, confidence High, signature_severity Informational, updated_at 2020_04_22;)",
  "rule.ruleset": "Emerging Threats",
  "rule.severity": 3,
  "rule.uuid": "2013504",
  "source.ip": "192.168.1.12",
  "source.port": 41934,
  "tags": [
    "alert",
    "_geoip_expired_database",
    "alert"
  ],
  "soc_id": "5mxY_pYBtNennHIu60sd",
  "soc_score": 2.003765,
  "soc_type": "",
  "soc_timestamp": "2025-05-23T18:12:35.925Z",
  "soc_source": "securityonion-rtulab:.ds-logs-suricata.alerts-so-2025.05.22-000012"
}
```

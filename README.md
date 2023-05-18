# Nokia Data Center Solutions

## Nokia SRLinux Ansible Collection

The Ansible Nokia SR Linux Collection includes a variety of Ansible content to help automate the management of Nokia SR Linux network appliances

This collection has been tested against Nokia SR Linux 22.x and above

## Getting Started


### 1. Create a Python virtual env with Python 3.8
`python3.8 -m venv virtual-ansible`
 
### 2. Clone the repo
`git clone link-to-be-updated`

### 3. Install requirements
Change the folder to `cd srlinux-ansible/` and install using the following command
`pip install -r requirements.txt`
 
### 4. Install Ansible SR Linux collection
`ansible-galaxy collection install .`

### 5. Config at SR Linux Node
The Nokia SR Linux Ansible Network modules communicate over the http connection, Make sure to enable it on the target nodes.
```
set / system json-rpc-server admin-state enable
set / system json-rpc-server network-instance mgmt
set / system json-rpc-server network-instance mgmt http
set / system json-rpc-server network-instance mgmt http admin-state enable
```

<!--start requires_ansible-->
## Ansible version compatibility
This collection has been tested against following Ansible versions: >=2.13.4

For collections that support Ansible 2.9 and beyond, please ensure you update your network_os to use the fully qualified collection name (for example, cisco.ios.ios). Plugins and modules within a collection may be tested with only specific Ansible versions. A collection may contain metadata that identifies these versions. PEP440 is the schema used to describe the versions of Ansible.

<!--end requires_ansible-->

### Supported connections
The Nokia SR Linux collection supports `JSON-RPC` connections.

## Included content
<!--start collection content-->
### Httpapi plugins
Name | Description
--- | ---
[nokia.srl.httpapi](http://example.com/repository/blob/main/docs/nokia.srl.httpapi_httpapi.rst)|HttpApi Plugin for devices supporting jsonrpc

### Modules
Name | Description
--- | ---
[nokia.srl.srl_acl_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_acl_interfaces_module.rst)|Manages attributes of srl acl_interfaces.
[nokia.srl.srl_acls](http://example.com/repository/blob/main/docs/nokia.srl.srl_acls_module.rst)|Manages attributes of srl acls.
[nokia.srl.srl_banner](http://example.com/repository/blob/main/docs/nokia.srl.srl_banner_module.rst)|Manages attributes of srl banner.
[nokia.srl.srl_bannernew](http://example.com/repository/blob/main/docs/nokia.srl.srl_bannernew_module.rst)|Manages attributes of srl bannernew.
[nokia.srl.srl_bgp_global](http://example.com/repository/blob/main/docs/nokia.srl.srl_bgp_global_module.rst)|Manages attributes of srl bgp_global.
[nokia.srl.srl_bgp_group](http://example.com/repository/blob/main/docs/nokia.srl.srl_bgp_group_module.rst)|Manages attributes of srl bgp_group.
[nokia.srl.srl_bgp_neighbor](http://example.com/repository/blob/main/docs/nokia.srl.srl_bgp_neighbor_module.rst)|Manages attributes of srl bgp_neighbor.
[nokia.srl.srl_command](http://example.com/repository/blob/main/docs/nokia.srl.srl_command_module.rst)|Manages attributes of srl command.
[nokia.srl.srl_config](http://example.com/repository/blob/main/docs/nokia.srl.srl_config_module.rst)|Manages attributes of srl config.
[nokia.srl.srl_gnmi_server](http://example.com/repository/blob/main/docs/nokia.srl.srl_gnmi_server_module.rst)|Manages attributes of srl gnmi_server.
[nokia.srl.srl_hostname](http://example.com/repository/blob/main/docs/nokia.srl.srl_hostname_module.rst)|Manages attributes of srl hostname.
[nokia.srl.srl_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_interfaces_module.rst)|Manages attributes of srl interfaces.
[nokia.srl.srl_irb_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_irb_interfaces_module.rst)|Manages attributes of srl irb_interfaces.
[nokia.srl.srl_isis](http://example.com/repository/blob/main/docs/nokia.srl.srl_isis_module.rst)|Manages attributes of srl isis.
[nokia.srl.srl_json_rpc_server](http://example.com/repository/blob/main/docs/nokia.srl.srl_json_rpc_server_module.rst)|Manages attributes of srl json_rpc_server.
[nokia.srl.srl_l2_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_l2_interfaces_module.rst)|Manages attributes of srl l2_interfaces.
[nokia.srl.srl_l3_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_l3_interfaces_module.rst)|Manages attributes of srl l3_interfaces.
[nokia.srl.srl_lacp](http://example.com/repository/blob/main/docs/nokia.srl.srl_lacp_module.rst)|Manages attributes of srl lacp.
[nokia.srl.srl_lacp_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_lacp_interfaces_module.rst)|Manages attributes of srl lacp_interfaces.
[nokia.srl.srl_lag_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_lag_interfaces_module.rst)|Manages attributes of srl lag_interfaces.
[nokia.srl.srl_lldp_global](http://example.com/repository/blob/main/docs/nokia.srl.srl_lldp_global_module.rst)|Manages attributes of srl lldp_global.
[nokia.srl.srl_lldp_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_lldp_interfaces_module.rst)|Manages attributes of srl lldp_interfaces.
[nokia.srl.srl_lo_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_lo_interfaces_module.rst)|Manages attributes of srl lo_interfaces.
[nokia.srl.srl_logging_global](http://example.com/repository/blob/main/docs/nokia.srl.srl_logging_global_module.rst)|Manages attributes of srl logging_global.
[nokia.srl.srl_network_instance](http://example.com/repository/blob/main/docs/nokia.srl.srl_network_instance_module.rst)|Manages attributes of srl network_instance.
[nokia.srl.srl_ntp_global](http://example.com/repository/blob/main/docs/nokia.srl.srl_ntp_global_module.rst)|Manages attributes of srl ntp_global.
[nokia.srl.srl_ospf](http://example.com/repository/blob/main/docs/nokia.srl.srl_ospf_module.rst)|Manages attributes of srl ospf.
[nokia.srl.srl_ospf_interfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_ospf_interfaces_module.rst)|Manages attributes of srl ospf_interfaces.
[nokia.srl.srl_prefix_lists](http://example.com/repository/blob/main/docs/nokia.srl.srl_prefix_lists_module.rst)|Manages attributes of srl prefix_lists.
[nokia.srl.srl_route_maps](http://example.com/repository/blob/main/docs/nokia.srl.srl_route_maps_module.rst)|Manages attributes of srl route_maps.
[nokia.srl.srl_snmp_server](http://example.com/repository/blob/main/docs/nokia.srl.srl_snmp_server_module.rst)|Manages attributes of srl snmp_server.
[nokia.srl.srl_static_routes](http://example.com/repository/blob/main/docs/nokia.srl.srl_static_routes_module.rst)|Manages attributes of srl static_routes.
[nokia.srl.srl_subinterfaces](http://example.com/repository/blob/main/docs/nokia.srl.srl_subinterfaces_module.rst)|Manages attributes of srl subinterfaces.
[nokia.srl.srl_system](http://example.com/repository/blob/main/docs/nokia.srl.srl_system_module.rst)|Manages attributes of srl system.
[nokia.srl.srl_user](http://example.com/repository/blob/main/docs/nokia.srl.srl_user_module.rst)|Manages attributes of srl user.
[nokia.srl.srl_vlans](http://example.com/repository/blob/main/docs/nokia.srl.srl_vlans_module.rst)|Manages attributes of srl vlans.
[nokia.srl.srl_vrf](http://example.com/repository/blob/main/docs/nokia.srl.srl_vrf_module.rst)|Manages attributes of srl vrf.

<!--end collection content-->


## Notes

1. The Nokia SR Linux Network Modules would build the config playbook as per the yang structure.
2. Make sure the playbooks follows the same JSON structure from the node using the command from node `info | as json`.
3. At playbooks, Dictionary are represented with `:` 
4. At playbooks, List are started/represnted with `-`
5. At cases where the dictionary is empty string, it is represented as `{ }` (curly brackets with empty string) 
6. With various data type, an examples
```
### Config snippet from the node in JSON

--{ + running }--[  ]--
A:srl2# info acl ipv4-filter tcp_allow | as json
{
  "acl": {
    "ipv4-filter": [                                 #ipv4-filter is list, so in the playbook the first items of the list would would start with '-' example: '- name:'
      {
        "name": "tcp_allow",
        "entry": [                                   #entry is list, so in the playbook the items would start with '-' example: '- sequence-id:'
          {
            "sequence-id": 1,
            "action": {
              "accept": {                           # accept is empty dictionary 
              }
            },
            "match": {                               #dictionary/nested-dictionary, these would add its items in generic 'key: value' fashion. 
              "protocol": "tcp",
              "source-port": {
                "value": "8082"
              }
            }
          }
        ]
      }
    ]
  }
}


### Playbooks in yaml format

---
- hosts: nokia

  tasks:
  - name: setting up acls
    nokia.srl.srl_acls:
      config:
        ipv4-filter:
        - name: tcp_allow
          entry:
            - sequence-id: '1'
              action:
                accept: { }
              match:
                protocol: 'tcp'
                source-port:
                  value: '8082'

```


## Installing this collection

You can install the Nokia SR Linux collection by cloning this repo with:
    ansible-galaxy collection install .

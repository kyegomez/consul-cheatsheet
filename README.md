# HashiCorp Consul Cheat Sheet

| Command / Tip | Description | Documentation |
|---------------|-------------|---------------|
| `consul agent -dev` | Start Consul in development mode. | [Consul Agent](https://www.consul.io/docs/agent) |
| `consul members` | List the members of a Consul cluster. | [Consul Members](https://www.consul.io/commands/members) |
| `consul join <address>` | Join a node to a Consul cluster. | [Consul Join](https://www.consul.io/commands/join) |
| `consul catalog services` | List all services registered with the Consul cluster. | [Catalog Services](https://www.consul.io/api-docs/catalog#list-services) |
| `consul catalog nodes -service=<name>` | List nodes associated with a given service. | [Catalog Nodes for Service](https://www.consul.io/api-docs/catalog#list-nodes-for-service) |
| `consul kv put <key> <value>` | Add or update a key-value pair. | [KV Put](https://www.consul.io/commands/kv/put) |
| `consul kv get <key>` | Retrieve the value of a key. | [KV Get](https://www.consul.io/commands/kv/get) |
| `consul watch -type=<type> <parameters>` | Watch for changes in Consul's state. | [Consul Watch](https://www.consul.io/commands/watch) |
| `consul snapshot save <file>` | Take a snapshot of the Consul server state. | [Snapshot Save](https://www.consul.io/commands/snapshot/save) |
| `consul snapshot restore <file>` | Restore a Consul server state from a snapshot. | [Snapshot Restore](https://www.consul.io/commands/snapshot/restore) |
| `consul acl bootstrap` | Bootstrap ACLs. Generates a management token. | [ACL Bootstrap](https://www.consul.io/commands/acl/bootstrap) |
| `consul acl policy create -name <name> -rules <rules>` | Create an ACL policy. | [ACL Policy Create](https://www.consul.io/commands/acl/policy#create) |
| `consul acl token create -description <desc> -policy-name <name>` | Create an ACL token with the specified policy. | [ACL Token Create](https://www.consul.io/commands/acl/token#create) |
| **Tip: Secure Consul** | Always enable ACLs for production environments to control access. | [ACL Guide](https://www.consul.io/docs/security/acl) |
| **Tip: Use Consul Connect** | For secure service-to-service communication, utilize Consul Connect. | [Consul Connect](https://www.consul.io/docs/connect) |
| **Tip: Datacenter Federation** | Use federation to enable service discovery and configurations across multiple Consul datacenters. | [Federation Guide](https://www.consul.io/docs/enterprise/federation) |
| **Tip: Monitoring and Metrics** | Leverage Consul's telemetry features for monitoring and performance metrics. | [Monitoring Consul](https://www.consul.io/docs/agent/telemetry) |
| **Tip: Disaster Recovery** | Regularly back up your Consul state and familiarize yourself with restore procedures. | [Disaster Recovery](https://www.consul.io/docs/commands/snapshot) |
| **Tip: Consul Template** | Use Consul Template for dynamic updates to configurations based on Consul's state. | [Consul Template](https://github.com/hashicorp/consul-template) |
| **Tip: Service Mesh Configurations** | Define service protocols in service definitions for L7 features in Consul Connect. | [Service Configuration](https://www.consul.io/docs/connect/configuration) |

This cheat sheet covers foundational commands and practices for working with Consul. For a more comprehensive guide and advanced topics, refer to the official [Consul Documentation](https://www.consul.io/docs).

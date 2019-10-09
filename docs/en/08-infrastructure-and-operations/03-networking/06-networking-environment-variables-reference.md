# Networking Environment Variables Reference

## Load Balancer Settings

```json
"loadBalancer": {
    "cdn": true,
    "targetPort": 3000,
    "customDomains": ["example.com"],
    "ssl": {
      "key": "...",
      "crt": "..."
    }
  }
```

## Private Network Settings

```json
{
  "id": "db",
  "ports": [
    {
      "port": 3400,
      "targetPort": 7000,
      "protocol": "TCP"
    },
    {
      "port": 9000,
      "targetPort": 8000,
      "protocol": "TCP",
      "external": true
    }
  ]
}
```

## Additional Information

* [Configuration via LCP JSON](../10-reference/02-configuration-via-lcp-json.md)
* [Adding Environment Variables](../../03-platform-overview/03-adding-environment-variables.md)
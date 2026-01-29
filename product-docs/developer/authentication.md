# Authentication

Authenticate with Kernel's API using access tokens.

## Overview

Kernel uses bearer token authentication for API access. Tokens are created in your account settings and included in API requests.

## Creating Tokens

### Personal Access Tokens

1. Log into Kernel
2. Go to **Settings** > **Security**
3. Click **API Tokens**
4. Click **Create Token**
5. Configure the token:
   - **Name**: Descriptive identifier
   - **Expiration**: When the token expires
   - **Scopes**: Permissions granted
6. Click **Create**
7. **Copy the token immediately** — it won't be shown again

### Token Scopes

| Scope | Permissions |
|-------|-------------|
| `read` | View constructs, parts, repositories |
| `write` | Create and modify content |
| `delete` | Remove content |
| `admin` | Workspace administration |

Request minimal scopes needed for your use case.

## Using Tokens

### HTTP Header

Include the token in the Authorization header:

```
Authorization: Bearer YOUR_TOKEN
```

### cURL Example

```bash
curl -X GET \
  -H "Authorization: Bearer YOUR_TOKEN" \
  -H "Content-Type: application/json" \
  https://kernel.asimov.com/api/v1/constructs
```

### Python Example

```python
import requests

headers = {
    "Authorization": f"Bearer {token}",
    "Content-Type": "application/json"
}

response = requests.get(
    "https://kernel.asimov.com/api/v1/constructs",
    headers=headers
)
```

### SDK Example

```python
from kernel import KernelClient

# Token passed to client
client = KernelClient(token="YOUR_TOKEN")

# Or use environment variable
# export KERNEL_TOKEN=your_token
client = KernelClient()  # Reads from KERNEL_TOKEN
```

## Token Management

### View Active Tokens

1. Go to **Settings** > **Security** > **API Tokens**
2. See list of your tokens
3. View last used date

### Revoke Tokens

1. Find the token in your list
2. Click **Revoke**
3. Confirm revocation
4. Token immediately stops working

### Token Expiration

Tokens expire based on their configured lifetime:
- 30 days (default)
- 90 days
- 1 year
- Custom expiration

Renew tokens before expiration to avoid disruption.

## Security Best Practices

### Storage

**Do:**
- Use environment variables
- Use secret management systems
- Store encrypted at rest

**Don't:**
- Commit tokens to code repositories
- Share tokens via email/chat
- Log tokens in application logs

### Environment Variables

```bash
# Set token in environment
export KERNEL_TOKEN="your_token_here"

# Use in code
import os
token = os.environ["KERNEL_TOKEN"]
```

### Secret Management

For production applications:
- AWS Secrets Manager
- HashiCorp Vault
- Azure Key Vault
- GCP Secret Manager

### Rotation

- Rotate tokens regularly
- Create new token before revoking old
- Update all applications using the token
- Revoke old token after migration

## Troubleshooting

### 401 Unauthorized

- Verify token is correct
- Check token hasn't expired
- Confirm token hasn't been revoked
- Ensure proper header format

### 403 Forbidden

- Token lacks required scope
- Resource not accessible to token owner
- Workspace permissions insufficient

### Token Not Working

1. Verify the token was copied completely
2. Check for extra whitespace
3. Confirm the token is for the correct environment
4. Test with a simple API call

## OAuth/SSO

*For enterprise integrations*

Contact sales@asimov.com for:
- SAML integration
- OAuth applications
- Custom authentication flows

## Next Steps

- [API Overview](api-overview.md) — Full API documentation
- [Common Operations](common-operations.md) — Example code
- [Account Settings](../settings/account-workspace.md) — Token management

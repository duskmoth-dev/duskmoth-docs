# API reference

All routes are relative to the server origin. Responses are JSON except the share-card image.

| Method | Route | Input / role |
|---|---|---|
| GET | /api/health | Service status; not proof that every provider is reachable |
| GET | /api/config | Readiness and configured transfer limits |
| POST | /api/intent | {message}; returns an intent, never executes it |
| POST | /api/screen | {sender, recipient}; sanctions only |
| POST | /api/activity | {address}; public chain balances and activity |
| POST | /api/score | {address, ts, signature}; ownership proof required |
| GET | /api/relayer/config | Current relayer fee and minimum configuration |

The RPC and relayer proxy routes are allowlisted infrastructure endpoints, not an authorization bypass.
The waitlist is unavailable until durable storage is implemented.
Keep provider keys on the server. Handle non-2xx, missing data, and timeouts explicitly.

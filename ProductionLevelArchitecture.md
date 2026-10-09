Google / GitHub / Username + Password
                 │
                 ▼
       Identity / Authentication
                 │
                 ▼
        JobPilot access token
          (RS256 + JWKS)
                 │
                 ▼
          API Gateway :8000
          ├── Verify JWT
          ├── Apply access policy
          ├── Rate limiting
          └── Route request
                 │
        ┌────────┼─────────┐
        ▼        ▼         ▼
     JobPilot  Jobs       AI
     Profile   Service    Service
        │        │         │
        └── Each validates token ──┘

# .github
All necessary information like design , architecture , flow etc will find place here 


                           ┌─────────────────────┐
                           │      JobPilot UI    │
                           │       React         │
                           └──────────┬──────────┘
                                      │
                                      ▼
                           ┌─────────────────────┐
                           │     API Gateway     │
                           │   Spring Cloud      │
                           │      Gateway        │
                           └──────────┬──────────┘
                                      │
              ┌───────────────────────┼────────────────────────┐
              │                       │                        │
              ▼                       ▼                        ▼
        ┌───────────┐           ┌────────────┐          ┌─────────────┐
        │ JobPilot  │           │ jobpilot-ai│          │ future      │
        │ Core      │           │            │          │ services    │
        └─────┬─────┘           └─────┬──────┘          └──────┬──────┘
              │                       │                        │
              │                       ▼                        │
              │                    Qdrant                      │
              │                       │                        │
              │                       ▼                        │
              │                    Gemini                       │
              │                                                │
              │                                      ┌─────────┴────────┐
              │                                      │                  │
              ▼                                      ▼                  ▼
          MongoDB                              Naukri/other       LinkedIn/other
                                               job providers      integrations

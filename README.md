# Weather Info API

## Features
- GET `/weather?city=<city>` → Returns JSON with temperature, humidity, description
- Dockerized
- GitHub Actions deploy to EC2

## Setup
1. Add `OPENWEATHER_API_KEY` in GitHub secrets.
2. Push code to main branch.
3. Workflow builds Docker image and deploys on EC2.

## Test
```bash
curl "http://<EC2_IP>:5000/weather?city=London"
```
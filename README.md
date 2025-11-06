# Dice Roller - Server

Azure Function App that provides random dice rolling service via HTTP API.

## Author
Salavuddin Shaik  
Lewis University  
Software Architecture and Design  
CPSC-61200-003

## AI Usage
This project was developed with assistance from Claude AI (Anthropic) for:
- Understanding Azure Function App deployment and configuration
- Implementing HTTP-triggered serverless function in Node.js
- Configuring CORS for cross-origin client requests
- Troubleshooting Azure Function App authentication and CORS policies
- Setting up proper response headers for API communication

## Description
This is the server-side component of a distributed dice roller system. The Azure Function:
- Accepts HTTP GET requests
- Generates random numbers between 1 and 6
- Returns plain text response
- Implements CORS to allow browser-based client requests

## Technologies
- Node.js
- Azure Function App
- HTTP Trigger
- CORS Headers

## Architecture
Service-Oriented Architecture (SOA) implementation:
- **Server**: Azure Function App (this repository)
- **Client**: Web interface hosted on Azure Static Website

## API Endpoint
```
GET https://dicerollerserver-dba2cjhhdbfhb5en.northcentralus-01.azurewebsites.net/api/roll-dice
```

Response: Plain text number (1-6)

## Client Repository
https://github.com/SalavuddinShaik/DiceRoller
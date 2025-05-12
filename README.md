# WhatsApp Cooking AI Assistant

An intelligent cooking assistant that integrates with WhatsApp to provide personalized recipe recommendations and cooking guidance.

## Features

- 🤖 AI-powered conversational system with multiple chef personalities
- 📱 WhatsApp Business API integration
- 🥘 Personalized recipe recommendations
- 👤 User profile management
- 📝 Ingredient tracking and management
- 🧠 Context-aware conversations
- 🛒 Smart grocery planning

## Project Structure

```
whatsapp_bot/
├── app/
│   ├── api/            # API routes and endpoints
│   ├── core/           # Core configuration and settings
│   ├── db/             # Database models and connection
│   ├── services/       # Business logic and services
│   ├── models/         # Pydantic models
│   └── utils/          # Utility functions
├── tests/              # Test files
├── .env               # Environment variables
├── requirements.txt   # Project dependencies
└── main.py           # Application entry point
```

## Setup Instructions

1. Clone the repository
2. Create a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with the following variables:
   ```
   MONGODB_URL=your_mongodb_url
   TWILIO_ACCOUNT_SID=your_twilio_sid
   TWILIO_AUTH_TOKEN=your_twilio_token
   OPENAI_API_KEY=your_openai_key
   WHATSAPP_NUMBER=your_whatsapp_number
   ```
5. Run the application:
   ```bash
   uvicorn main:app --reload
   ngrok http 8000
   copy url to twilio webhook
   ```

## API Documentation

Once the server is running, visit `http://localhost:8000/docs` for the interactive API documentation.

## Environment Variables

- `MONGODB_URL`: MongoDB connection string
- `TWILIO_ACCOUNT_SID`: Twilio Account SID
- `TWILIO_AUTH_TOKEN`: Twilio Auth Token
- `OPENAI_API_KEY`: OpenAI API Key
- `WHATSAPP_NUMBER`: Your WhatsApp Business number
- `JWT_SECRET_KEY`: Secret key for JWT token generation
- `ALGORITHM`: Algorithm for JWT token generation

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

MIT License 
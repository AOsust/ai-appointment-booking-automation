# AI Appointment Booking Automation

Automatizacija procesa rezervacije termina primjenom n8n platforme i umjetne inteligencije.

Projekt je razvijen kao završni rad na Tehničkom veleučilištu u Zagrebu. Sustav povezuje AI agenta, n8n workflow, Google Sheets i Cal.com API kako bi automatizirao proces od korisničkog zahtjeva do rezervacije termina.

## Demo

[▶️ Pogledaj video demonstraciju projekta](https://youtu.be/yGMoujFaq_Y)


## About the Project

The project presents an automated appointment booking system based on an AI conversational agent and workflow automation.

The system allows the user to communicate using natural language, provide the required information, select a service and choose an available appointment.

Behind the conversational interface, n8n coordinates communication between the AI agent and external services.

The workflow retrieves available appointment slots, processes the user's selection and creates the booking through the Cal.com API.

Google Sheets is used for storing and updating relevant user and booking data.


## Main Features

- AI-powered conversational interface
- Automated appointment booking
- Appointment availability checking
- Service selection
- User data collection
- Integration with Cal.com
- Google Sheets data storage
- REST API communication
- HTTP requests
- JSON data processing
- Automated booking confirmation
- Email appointment reminder
- Error handling for unsuccessful booking attempts
- Time and timezone processing

## System Architecture

                    User
                      │
                      ▼
              AI Conversational Agent
                      │
                      ▼
                     n8n
                      │
          ┌───────────┼───────────┐
          │           │           │
          ▼           ▼           ▼
    Google Sheets   Cal.com     API Services
          │           │
          │           ▼
          │     Availability
          │           │
          │           ▼
          │       Booking
          │
          ▼
      Stored Data
                      │
                      ▼
              Confirmation
                      │
                      ▼
               Email Reminder

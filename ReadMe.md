# 🔗 URL Shortener with Go, Fiber, and Redis 🚀

This project is a URL shortener service built using Go, Fiber web framework, and Redis for data storage.

## 🌟 Features

- 🔗 Shorten long URLs
- 🎨 Custom short URLs
- ⏳ URL expiration
- 🔒 Rate limiting
- 🔄 URL redirection

## 🛠️ Tech Stack

- 🐹 Go
- 🚀 Fiber web framework
- 🗄️ Redis
- 🐳 Docker & Docker Compose

## 🚀 Getting Started

### Prerequisites

- 🐳 Docker and Docker Compose installed

### Running the application

1. Clone the repository  `git clone https://github.com/inagib21/shorten-url-fiber-redis.git`
2. Navigate to the project directory
3. Run the following command:

docker-compose up --build


The API will be available at `http://localhost:3000`

## 🔧 API Endpoints

### POST /api/v1
Shorten a URL

Request body:

json
{
"url": "https://example.com",
"custom_short": "optional-custom-short",
"expiry": 24
}


### GET /:url
Redirect to the original URL

## 🧪 Environment Variables

Create a `.env` file in the `api` directory with the following variables:



### GET /:url
Redirect to the original URL

## 🧪 Environment Variables

Create a `.env` file in the `api` directory with the following variables:
APP_PORT=:3000
DB_ADDR=db:6379
DB_PASS=
API_QUOTA=10
DOMAIN=localhost:3000

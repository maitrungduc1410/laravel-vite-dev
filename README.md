# Laravel Dev Demo

Demo Laravel + Vite hot reload using Docker for development

Install dependencies:
```
# MacOS + Linux
docker run --rm -v $(pwd):/app -w /app prooph/composer:8.2 install

docker run --rm -v $(pwd):/app -w /app prooph/composer:8.2 dump-autoload

docker run --rm -v $(pwd):/app -w /app node:20-alpine npm install

# If Windows see below:

# Git bash
docker run --rm -v "/$(pwd)":/app -w //app prooph/composer:8.2 install

docker run --rm -v "/$(pwd)":/app -w //app prooph/composer:8.2 dump-autoload

docker run --rm -v "/$(pwd)":/app -w //app node:20-alpine npm install

# PowerShell
docker run --rm -v "$(pwd):/app" -w /app prooph/composer:8.2 install

docker run --rm -v "$(pwd):/app" -w /app prooph/composer:8.2 dump-autoload

docker run --rm -v "$(pwd):/app" -w /app node:20-alpine npm install

# Command Prompt
docker run --rm -v "%cd%:/app" -w /app prooph/composer:8.2 install

docker run --rm -v "%cd%:/app" -w /app prooph/composer:8.2 dump-autoload

docker run --rm -v "%cd%:/app" -w /app node:20-alpine npm install

```

Start project:
```
docker compose up -d
```

Access from browser: `http://localhost:8000`
# leavenull_bot
A lightweight open-source solution for Telegram to show info about users who have just left the group.

## Usage
You can run the bot using Docker Compose with the pre-built [image available on Docker Hub](https://hub.docker.com/r/endergofficial/leavenull_bot):

1. Create a `docker-compose.yml` file in your project directory:

```yaml
services:
  leavenull_bot:
    image: endergofficial/leavenull_bot:latest
    restart: always
    environment:
      - TOKEN=your_bot_token_here
```

2. Replace `your_bot_token_here` with your actual Telegram bot token.
3. Start the container in detached mode:

```bash
docker compose up -d
```

## Configuration
All configuration is managed through environment variables:

| Variable    | Type  | Default        | Description          |
| :---:       | :---: | :---:          | :---                 |
| `TOKEN`     | `str` | Required       | Telegram Bot token   |
| `LOG_LEVEL` | `int` | `logging.INFO` | Logging level        |

## Links
- GitHub repository: https://github.com/artkiselev704/leavenull_bot
- Docker Hub repository: https://hub.docker.com/r/endergofficial/leavenull_bot

# syntax=docker/dockerfile:1

FROM python:3.12-slim

# Install FFmpeg
RUN --mount=type=cache,target="/var/cache/apt",sharing=locked \
    --mount=type=cache,target="/var/lib/apt/lists",sharing=locked \
    apt-get update && \
    apt-get upgrade -y && \
    apt-get install --no-install-recommends -y \
    build-essential \
    # psycopg dependencies
    libpq-dev \
    ffmpeg && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["python3"]

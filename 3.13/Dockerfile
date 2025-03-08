# syntax=docker/dockerfile:1

# hadolint global ignore=DL3008

FROM python:3.13-slim

# Install FFmpeg
RUN --mount=type=cache,target="/var/cache/apt",sharing=locked \
    --mount=type=cache,target="/var/lib/apt/lists",sharing=locked \
    apt-get update && \
    apt-get upgrade -y && \
    apt-get install --no-install-recommends -y \
    # psycopg dependencies
    libpq-dev \
    # ffmpeg dependencies
    ffmpeg \
    # libmagic
    libmagic1 && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*

CMD ["python3"]

# Lab 2: Containers with Docker

Starting code for **Lab 2** of the course *Containers & Orchestration* (Howest MCT, 2026-2027).
The assignment itself is on Leho: 🟢 Praktijk, Lab 2.

## What is in this repository

| Directory | Contents |
|---|---|
| `web/` | Empty. You build the Flask front-end here yourself in part 1. |
| `web_new/` | The full front-end code for part 2. Copy it into `web/` when the lab asks for it. No Dockerfile: you bring your own from part 1. |
| `api/` | The FastAPI backend, with its Dockerfile and `prestart.sh`. |
| `nginx/` | The Nginx web server that sits in front of the front-end. |

## Before you start

- Log in to Docker Hub once with `docker login`. Anonymous pulls are limited to 100 per 6 hours per IP address, and everyone in the classroom shares one address.
- Commit along the way, not only at the end.

## Part 2: switching to the full front-end

When the lab tells you to, replace the contents of `web/` with the contents of `web_new/`, but **keep your own Dockerfile**.
Then check whether your Dockerfile still works: where is `requirements.txt` now, and which module does `app.ini` start?
Delete `web_new/` afterwards.

## Changes

- 28/09/2026: prepared for 2026-2027 and Classroom 50. Nginx base image updated to `nginx:1.30-alpine`. The Dockerfile in `web_new/` was removed: writing it is part of the lab. `web/` no longer ignores its contents, so your part 1 work is committed.
- 17/03/2025: updates to `api/app/config.py` and `api/app/schemas/user.py`. The `.zip` file was replaced by `web_new/`.

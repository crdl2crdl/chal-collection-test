FROM python:slim AS app

FROM pwn.red/jail
COPY --from=app / /srv
COPY misc_random_flags.py ./srv/app/run
COPY flag.txt ./srv/app/flag.txt
RUN chmod +x /srv/app/run
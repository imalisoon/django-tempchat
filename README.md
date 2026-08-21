# tempchat built in Django

Web chat app with temporary timed chats.

# Functionalities (WIP)

- Authentication/Authorization
- E2EE ecryptation messages
- Real-Time chats between users
- Temporary time chats (15m)
- Invite/accetpt system users for chatting
- Add users to contact list

# Run locally

1. First, get the project.

```bash
git clone https://github.com/imalisoon/django-tempchat.git
cd django-tempchat
```

2. Next, set up the Python environment and install deps.

```bash
python -m venv .venv
source .venv/bin/activate
```
```bash
# install dependencies
pip install dev-requirements.txt
```

3. Rename the `example.env` to `.env`, generate the secret key using the script `scripts/generate-secret-key.py` and paste on the file.

```bash
mv example.env .env

python scripts/generate-secret-key.py
```
```bash
# .env

SECRET_KEY=
...
```
4. Finally, set up database and run the project.

```bash
python manage.py migrate

python manage.py runserver
```

Nice, access the `127.0.0.1:8000` address.

# License

under [MIT](./LICENSE)
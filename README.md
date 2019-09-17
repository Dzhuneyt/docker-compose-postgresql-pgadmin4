# PostgreSQL and pgAdmin4, powered by Docker Compose

A simple Docker Compose stack with 2 services:
- **PostgreSQL** database with mounted volume (data is persisted)
- **pgAdmin4** to administer the database through the UI (on a port defined in .env)

---

### Getting started

1. Clone the repo
2. Copy .env-dist to .env and edit it. Configure the pgAdmin4 port
3. `docker-compose up`
4. Open `http://localhost:[pgAdmin4-port-from-step-2]`
---

### Environment variables (.env):

* **PGADMIN_PORT** - which port will pgAdmin4 be accessible from. After starting the stack, open `http://localhost:${PGADMIN_PORT}`
* **PGADMIN_DEFAULT_USERNAME** - The username to use to login to pgAdmin4
* **PGADMIN_DEFAULT_PASSWORD** - The password for the above username
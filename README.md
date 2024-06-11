version: '3'
services:
  postgres:
    image: postgres:latest
    environment:
      POSTGRES_DB: mydatabase
      POSTGRES_USER: antonov421
      POSTGRES_PASSWORD: Vanya1810
    ports:
      - "5432:5432"

  pgadmin:
    image: dpage/pgadmin4
    environment:
      PGADMIN_DEFAULT_EMAIL: antonov421@example.com
      PGADMIN_DEFAULT_PASSWORD: Dasha989
    ports:
      - "80:80"

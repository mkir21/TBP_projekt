# Bud-dy

Aplikacija za upravljanje biljkama, podsjetnicima, događajima i mjerenjima.

## Zahtjevi

- Python 3.8+
- PostgreSQL
- virtualenv (preporučeno)

## Instalacija

# Klonirajte repozitorij:

git clone <repo-url>
cd <repo-root>

# Postavite virtualno okruženje:

python -m venv venv
source venv/bin/activate

# Instalirajte ovisnosti:
pip install -r requirements.txt

# Baza podataka
## Kreirajte bazu i korisnika ili prilagodite ENV varijable:
createdb biljke
psql biljke < baza.sql

## (Opcionalno) Postavite ENV varijable za konekciju:
Postavite ENV varijable za konekciju:
export DB_NAME=biljke
export DB_USER=korisnik
export DB_PASSWORD=lozinka
export DB_HOST=localhost
export DB_PORT=5432

# Pokretanje
cd projekt_code
python main.py         

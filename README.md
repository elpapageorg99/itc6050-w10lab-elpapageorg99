" ITC 6050 - Week 1 Lab" 

We run Postgres in Docker instead of installing it directly because Docker containers are portable, isolated, and reproducible — ensuring the same environment works identically on every machine without conflicts with local system settings.

What did dlt do for us?

Schema inference — automatically detected column types from the JSON response without us defining them manually.
Pagination handling — we only wrote the loop; dlt managed state and incremental loading.
Database loading — wrote the data directly to Postgres without us writing a single INSERT or SQLAlchemy model.
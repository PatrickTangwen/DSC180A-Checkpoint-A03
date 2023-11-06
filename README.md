# DSC180A-Checkpoint-A03

Command for createing psql databse:
```
psql
CREATE DATABASE med_dash;
\c med_dash
```

```
CREATE TABLE patient1_daily_hr (
    timestamp TIMESTAMP WITH TIME ZONE,
    bpm INTEGER,
    quality TEXT,
    source TEXT,
    restorative BOOLEAN
);
```

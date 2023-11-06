# DSC180A-Checkpoint-A03-Data_Integration

This week, we are starting to work on creating a local database to store patient data. Below is the command for the creation process.<br>
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

```
\COPY patient1_daily_hr FROM '/pathto/patient_1_daily_hr.csv' WITH (FORMAT csv, HEADER true, DELIMITER ',');
```

```
SELECT COUNT(*) FROM patient1_daily_hr;
```

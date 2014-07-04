# Abfragen
```sql
SELECT F.Name
FROM Studio S, Film F
WHERE F.Genre = 'Action' 
      AND F.Studio = S.ID
```

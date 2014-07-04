# Abfragen
//Start der Abfrage
//Gib alle Action Filme an welche in Hollywood gedreht wurden.
```sql
SELECT F.Name
FROM Studio S, Film F
WHERE F.Genre = 'Action' 
      AND F.Studio = S.ID
```
//Ende der Abfrage

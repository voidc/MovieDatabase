# Abfragen

Alle Romantik Filme, in denen deutsche Schauspieler mitspielen:
```sql
SELECT F.Titel, P.Name
FROM FILM F, PERSON P, IST_DARSTELLER_IN IDI
WHERE IDI.Film = F.ID
  AND IDI.Person = P.ID
  AND F.Genre = "Romantik"
  AND P.Nationalitaet = "deutsch"
```

Gib alle Action Filme an welche in Hollywood gedreht wurden.
```sql
SELECT F.Name
FROM Studio S, Film F
WHERE F.Genre = 'Action' 
  AND F.Studio = S.ID
  AND F.Ort = "Hollywood"
```

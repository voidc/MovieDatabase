# Abfragen

Alle Romantik Filme, in denen deutsche Schauspieler mitspielen:
```sql
SELECT F.Titel, P.Name
FROM FILM F, PERSON P, IST_DARSTELLER_IN IDI
WHERE IDI.Film = F.ID
  AND IDI.Person = P.ID
  AND F.Genre = "Romantik"
  AND P.Nationalität = "deutsch"
```

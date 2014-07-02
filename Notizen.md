# Notizen

### Film:
* ID
* Titel
* Orginaltitel
* Erscheinungsjahr
* FSK
* Laufzeit
* Metascore
* Genre
* Kurzbeschreibung
* Budget
* Einspielergebnisse
* Studio
* Director ref Person
* Writer

### IstDarstellerIn
* Film ref Film.ID
* Person ref Person.ID

### Person
* ID
* Name
* Nationalität
* Geburtsdatum
* Oscars

### FilmAusgezeichnetMit
* Film ref Film.ID
* Auszeichnung ref Auszeichnung.ID

### PersonAusgezeichnetMit
* Person ref Person.ID
* Auszeichnung ref Auszeichnung.ID

### Auszeichnung
* ID
* Name
* Typ
* Verleihungsdatum

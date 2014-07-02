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
* Studio ref Studio.ID
* Director ref Person.ID
* Writer ref Person.ID

### IstDarstellerIn
* Film ref Film.ID
* Person ref Person.ID
* Rolle
* Gage

### Person
* ID
* Name
* Nationalität
* Geburtsdatum

### Studio
* ID
* Name
* Ort

### FilmAusgezeichnetMit
* Film ref Film.ID
* Auszeichnung ref Auszeichnung.ID
* Verleihungsdatum
* Verleiher

### PersonAusgezeichnetMit
* Person ref Person.ID
* Auszeichnung ref Auszeichnung.ID
* Verleihungsdatum
* Verleiher

### Auszeichnung
* ID
* Name
* Typ

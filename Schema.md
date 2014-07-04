# Schema

*kursiv*: Fremdschlüssel  
**fett**: Primärschlüssel

FILM{  
  **ID**: INTEGER,  
  Titel: VARCHAR(50),  
  Orginaltitel: VARCHAR(50),  
  Erscheinungsjahr: DATE,  
  FSK: INTEGER,  
  Laufzeit: TIME,  
  Metascore: INTEGER,  
  Genre: VARCHAR(30),  
  Kurzbeschreibung: VARCHAR(1000),  
  Budget: INTEGER,  
  Einspielergebnisse: INTEGER,  
  *Studio*: INTEGER,  
  *Director*: INTEGER,  
  *Writer*: INTEGER  
}  
PERSON{  
  **ID**: INTEGER,  
  Name: VARCHAR(30),  
  Nationalitaet: VARCHAR(30),  
  Geburtsdatum: DATE  
}  
STUDIO{  
  **ID**: INTEGER,  
  Name: VARCHAR(30),  
  Ort: VARCHAR(30)  
}  
AUSZEICHNUNG{  
  **ID**: INTEGER,  
  Name: VARCHAR(30),  
  Typ: VARCHAR(30)  
}  
IST_DARSTELLER_IN{  
  ***Film***: INTEGER,  
  ***Person***: INTEGER,  
  Rolle: VARCHAR(30),  
  Gage: INTEGER  
}  
FILM_AUSGEZEICHNET_MIT{  
  ***Film***: INTEGER,  
  ***Auszeichnung***: INTEGER,  
  Verleihungsdatum: DATE,  
  Verleiher: VARCHAR(30)  
}  
PERSON_AUSGEZEICHNET_MIT{  
  ***Person***: INTEGER,  
  ***Auszeichnung***: INTEGER,  
  Verleihungsdatum: DATE,  
  Verleiher: VARCHAR(30)  
}



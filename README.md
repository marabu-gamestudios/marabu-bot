# Marabu Bot v.5 Dokumentation


## Inhaltsverzeichnis

- [To-Do-Liste](#to-do-liste)
  - [Befehl: To-Do-Liste anzeigen](#befehl-todo_anzeigen)
  - [Befehl: Punkt zur To-Do-Liste hinzufügen](#befehl-todo_adden)
  - [Befehl: Punktstatus ändern](#befehl-todo_status)
  - [Befehl: Punkt aus der To-Do-Liste entfernen](#befehl-todo_entfernen)
  - [Befehl: To-Do-Liste löschen](#befehl-todo_löschen)

- [Ideenwand](#ideenwand)
  - [Befehl: Idee zur Ideenwand hinzufügen](#befehl-idee_adden)
  - [Befehl: Idee von der Ideenwand lesen](#befehl-idee_lesen)
  - [Befehl: Idee von der Ideenwand löschen](#befehl-idee_löschen)
  - [Befehl: Ideenwand anzeigen](#befehl-ideen_anzeigen)
  - [Befehl: Ideenwand löschen](#befehl-ideen_löschen)

- [Chatbereinigung](#chatbereinigung)
  - [Befehl: Chatbereinigung](#befehl-chat_löschen)

- [Ausrufe](#ausrufe)
  - [Befehl: Ausruf hinzufügen](#befehl-ausruf_hinzufügen)
  - [Befehl: Ausrufe anzeigen](#befehl-ausrufe_anzeigen)

- [Musikbot](#musikbot)
  - [Befehl: YouTube-Video abspielen](#befehl-musik_play)
  - [Befehl: Radiosender anzeigen](#befehl-radio_list)
  - [Befehl: Radiosender abspielen](#befehl-radio_play)
  - [Befehl: Musik stoppen](#befehl-musik_stop)
  


## To-Do-Liste<a name="to-do-liste"></a>

### Befehl: To-Do-Liste anzeigen<a name="befehl-todo_anzeigen"></a>

```
/todo_anzeigen
```

Dieser Befehl zeigt die aktuelle To-Do-Liste im Discord-Chat an. Die Liste wird in einem Embed formatiert und in drei Spalten unterteilt: "Zu erledigen", "In Arbeit" und "Erledigt".

### Befehl: Punkt zur To-Do-Liste hinzufügen<a name="befehl-todo_adden"></a>

```
/todo_adden bereich:value aufgabe:value
```

Mit diesem Befehl kann ein neuer Punkt zur To-Do-Liste hinzugefügt werden. Die Aufgabe wird mit Angabe des Bereichs und der Beschreibung erstellt. Der Autor der Aufgabe wird automatisch erfasst.

**Parameter:**
- `bereich`: Der Bereich, für den die Aufgabe erledigt werden soll.
- `aufgabe`: Die Beschreibung der Aufgabe, die hinzugefügt werden soll.

### Befehl: Punktstatus ändern<a name="befehl-todo_status"></a>

```
/todo_status index:value column:value
```

Dieser Befehl ermöglicht es, den Status eines Punktes in der To-Do-Liste zu ändern und ihn in eine andere Spalte zu verschieben. Die Spalten sind "Zu erledigen", "In Arbeit" und "Erledigt".

**Parameter:**
- `index`: Die Nummer der Aufgabe, deren Status geändert werden soll.
- `column`: Die Spalte, in die die Aufgabe verschoben werden soll ('zu_erledigen', 'in_arbeit', 'erledigt').

### Befehl: Punkt aus der To-Do-Liste entfernen<a name="befehl-todo_entfernen"></a>

```
/todo_entfernen index:value
```

Mit diesem Befehl kann ein Punkt aus der To-Do-Liste entfernt werden, indem die Nummer des Punktes angegeben wird.

**Parameter:**
- `index`: Die Nummer der Aufgabe, die entfernt werden soll.

### Befehl: To-Do-Liste löschen<a name="befehl-todo_löschen"></a>

```
/todo_löschen password:value
```

Dieser Befehl löscht die gesamte To-Do-Liste. Es ist ein Passwort erforderlich, um die Liste zu löschen.

**Parameter:**
- `password`: Das Passwort zum Löschen der Liste.

## Ideenwand<a name="ideenwand"></a>

### Befehl: Idee zur Ideenwand hinzufügen<a name="befehl-idee_adden"></a>

```
/idee_adden title:value idea:value
```

Dieser Befehl ermöglicht es, eine neue Idee zur Ideenwand hinzuzufügen. Die Idee wird mit einer Überschrift und einer ausführlichen Beschreibung erstellt.

**Parameter:**
- `title`: Die Überschrift der Idee.
- `idea`: Die vollständige Beschreibung der Idee.

Continuing from the last section:

### Befehl: Idee von der Ideenwand lesen<a name="befehl-idee_lesen"></a>

```
/idee_lesen idea_number:value
```

Mit diesem Befehl kann eine spezifische Idee von der Ideenwand abgerufen und im Discord-Chat angezeigt werden.

**Parameter:**
- `idea_number`: Die Nummer der Idee, die abgerufen werden soll.

### Befehl: Idee von der Ideenwand löschen<a name="befehl-idee_löschen"></a>

```
/idee_löschen idea_number:value
```

Mit diesem Befehl kann eine Idee von der Ideenwand gelöscht werden.

**Parameter:**
- `idea_number`: Die Nummer der Idee, die gelöscht werden soll.

### Befehl: Ideenwand anzeigen<a name="befehl-ideen_anzeigen"></a>

```
/ideen_anzeigen
```

Dieser Befehl zeigt die gesamte Ideenwand im Discord-Chat an.

### Befehl: Ideenwand löschen<a name="befehl-ideen_löschen"></a>

```
/ideen_löschen password:value
```

Dieser Befehl löscht die gesamte Ideenwand.

**Parameter:**
- `password`: Das Passwort zum Löschen der Ideenwand.

## Chatbereinigung<a name="chatbereinigung"></a>

### Befehl: Chatbereinigung<a name="befehl-chat_löschen"></a>

```
/chat_löschen
```

Mit diesem Befehl können Nachrichten im Chat gelöscht werden. Dieser Befehl sollte nur von Administratoren verwendet werden.

## Ausrufe<a name="ausrufe"></a>

### Befehl: Ausruf hinzufügen<a name="befehl-ausruf_hinzufügen"></a>

```
/ausruf_hinzufügen channel:value times:value interval:value message:value
```

Mit diesem Befehl können automatische Ausrufe in einem bestimmten Kanal erstellt werden.

**Parameter:**
- `channel`: Der Kanal, in dem der Ausruf erfolgen soll.
- `times`: Die Anzahl der Wiederholungen des Ausrufs.
- `interval`: Das Zeitintervall zwischen den Wiederholungen (in Minuten).
- `message`: Die Nachricht, die in den Ausrufen gesendet werden soll.

### Befehl: Ausrufe anzeigen<a name="befehl-ausrufe_anzeigen"></a>

```
/ausrufe_anzeigen
```

Dieser Befehl zeigt alle aktuellen Ausrufe an.

## Musikbot<a name="musikbot"></a>

### Befehl: YouTube-Video abspielen<a name="befehl-musik_play"></a>

```
/musik_play youtube_url:value
```

Mit diesem Befehl kann ein YouTube-Video in einem Sprachkanal abgespielt werden.

**Parameter:**
- `youtube_url`: Die URL des YouTube-Videos, das abgespielt werden soll.

### Befehl: Radiosender anzeigen<a name="befehl-radio_list"></a>

```
/radio_list
```

Dieser Befehl zeigt alle verfügbaren Radiosender an, die vom Musikbot unterstützt werden.

### Befehl: Radiosender abspielen<a name="befehl-radio_play"></a>

```
/radio_play radio_position:value radio_name:value
```

Mit diesem Befehl kann ein Radiosender in einem Sprachkanal abgespielt werden.

**Parameter:**
- `radio_position`: Die Position des Radiosenders in der Liste der verfügbaren Radiosender.
- `radio_name`: Der Name des Radiosenders.

### Befehl: Musik stoppen<a name="befehl-musik_stop"></a>

```
/musik_stop
```

Dieser Befehl stoppt die Wiedergabe von Musik oder Radiosendern im Sprachkanal.


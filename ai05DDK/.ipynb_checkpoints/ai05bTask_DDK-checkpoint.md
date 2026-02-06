# API Query Building Assignment
---

## USGS Earthquake Queries

### Query 1: Looking for earthquakes that are greater than 6.0 in magnitude, and looking for only 20 results, instead of possible hundred entries.
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=6.0&limit=20
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minmagnitude
- `parameter3`: limit

**Result:** [Brief description of what JSON data you got back - how many earthquakes? what magnitude range? etc.]

---

### Query 2: [Describe what you're searching for]
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=2.0&maxmagnitude=3.0&limit=10
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minmagnitude
- `parameter3`: maxmagnitude

**Result:** [Brief description of what JSON data you got back]

---

### Query 3: [Describe what you're searching for]
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minlatitude=0.58&maxlatitude=29.76&limit=10
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minlatitude
- `parameter3`: maxlatitude

**Result:** [Brief description of what JSON data you got back]

---

## Open Library Queries

### Query 4: [Describe what you're searching for]
**URL:**
```
https://openlibrary.org/search.json?title=Astronomy&limit=10
```

**Parameters used:**
- `parameter1`: title
- `parameter2`: limit

**Result:** [Brief description of what JSON data you got back - how many books found? titles? authors?]


### Query 5: [Describe what you're searching for]
**URL:**
```
https://openlibrary.org/search.json?author=alan+gratz&limit=5
```

**Parameters used:**
- `parameter1`: author
- `parameter2`: [explanation]

**Result:** [Brief description of what JSON data you got back - how many books found? titles? authors?]

### Query 6: [Describe what you're searching for]
**URL:**
```
https://openlibrary.org/search.json?subject=history&limit=5
```

**Parameters used:**
- `parameter1`: subject
- `parameter2`: [explanation]

**Result:** [Brief description of what JSON data you got back - how many books found? titles? authors?]
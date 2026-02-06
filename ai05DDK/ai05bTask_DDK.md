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
- `parameter2`: minmagnitude (setting a minimum limit to follow)
- `parameter3`: limit (limiting how many entries can be seen)

**Result:** Turns out, there wasn't enough entries for the limit to be needed, as only 8 entries showed up, with majority of them turning out to be located in the Asian/Oceaniac areas.

---

### Query 2: Specifically searching for earthquakes between a magnitude of 2 and 5, requesting earthquakes that aren't too weak, but still somewhat strong.
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minmagnitude=2.0&maxmagnitude=5.0
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minmagnitude (getting earthquakes that are greater than or equal to 2.0, since we dont want weak sauce earthquakes.)
- `parameter3`: maxmagnitude (determining the max magnitude so that we won't get any earthquakes stronger than 5.0)

**Result:** There was a lot of entries, in comparison to the last url. In addition, just from skimming around a little bit, majority of the entries are located in United States.

---

### Query 3: Looking for earthquakes starting from slightly above the equator, and stopping at Cairo, only looking at that region of Earth, in terms of the latitude.
**URL:**
```
https://earthquake.usgs.gov/fdsnws/event/1/query?format=geojson&minlatitude=0.58&maxlatitude=29.76
```

**Parameters used:**
- `format`: geojson
- `parameter2`: minlatitude (this determines the minimum height of where we are looking, and it stops at just slightly above the equator) 
- `parameter3`: maxlatitude (the max height of where we are looking, so this stops at Cairo)

**Result:** As expected, if you try to search for a nation/country that is below the equator, they don't show up because we are targetting a specific region of the Earth. This also applies to nations who are above the city of Cairo, as they are not inside of the region we are targetting.

---

## Open Library Queries

### Query 4: Searching for books that have the keyword: "Astronomy", in the titles of the books, but only looking for around 10 of them.
**URL:**
```
https://openlibrary.org/search.json?title=Astronomy&limit=10
```

**Parameters used:**
- `parameter1`: title (searching for a keyword in the title, that being Astronomy)
- `parameter2`: limit (limiting # of entries)

**Result:** As expected, only 10 entries showed up because that is the limit we set. What's also intriguing, is that a lot of the entries just blatantly have "Astronomy" as their titles, instead of having extra words on top of that.


### Query 5: Looking for books created by Alan Gratz.
**URL:**
```
https://openlibrary.org/search.json?author=alan+gratz&limit=5
```

**Parameters used:**
- `parameter1`: author (without this, we would get books that might have a similar title to what he has written, but it wouldn't be written by him.)
- `parameter2`: limit (Alan Gratz may have tons of books, so it's best to only look at five of them.)

**Result:** The books we are given from the dataset are some of the greatest hits that he has, like Refugee, and Projekt 1065.

### Query 6: Books that are related to the subject of history
**URL:**
```
https://openlibrary.org/search.json?subject=history&limit=5
```

**Parameters used:**
- `parameter1`: subject (this is what allows us to look for books that have the subject of history tied to them)
- `parameter2`: limit (again, the possibility of having thousands of books related to history is very possible, so a limit is needed)

**Result:** Some of the books that are in the dataset turn out to have quite a lot of languages attached to them, and one of them is even titled in Russian Cyrillic as well. It seems like the history books are more international.
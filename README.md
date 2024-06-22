# Black Marketeer Search
GUI for parsing the X4: Foundations Game Save to allow easier search for Black Marketer vendors.

After loading the game save and selecting the sector, tool shows the stations in the sector and the status of black marketeers on them:
- Active (black marketeer unlocked)
- Inactive (black marketeer still locked)
- N/A (black marketeer not available on the station)

---

X4: Foundations is the registered trademark of the EGOSOFT GmbH 

## Development notes

## Run Shady Search - no debug
```bash
./gradlew clean build bootRun
```

## Run Shady Search  with debug
```bash
./gradlew clean build bootRun -PjvmArgs="-agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=5005"
```
```bash
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=5005 -jar .\build\libs\shady-search-0.0.2-SNAPSHOT.jar
```


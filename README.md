# Guacamole | Guild Ranks

This project is created to automate the rank system we have in the guild Guacamole in WoW TBC real Benediction.  
These ranks affect the priority when rolling loot. 

# How the rank system works in Guacamole
Manual (This is approved by officers)
* Creates/Maintains Good environment
* Is a good player (does mechanics in fights for her/his role, measures her/his agro, decent parses in warcraft logs, special armor sets for mechanics, has enchants and gems in armor equiped)
* Almost no lag (to avoid accidental wipes for net issues)
* Hears the raid in discord

Automatic (This project)
* Uses consumables (elixirs/flask, scrolls, temporary weapon enchant, food)
* Attendance percentage in "mandatory" raids for the last 3 weeks

Notes
* If a player stays in bench, will have attendance for a maximum of 33% of the total attendance in the last 3 weeks
* If a player goes with an alter, attendace will count as well

# Measurement

| rank       | good environment | good player | almost no lag | uses discord | consumables | attendance |
|------------|------------------|-------------|---------------|--------------|-------------|------------|
| 😎Exaltado | 1                | 1           | 1             | 1            |>250         |>75%        |
| ⚔️Estable  | 0                | 1           | 1             | 1            |>250         |>60%        |
| 🌓5050     | 0                | 0           | 0             | 0            |0            |>33%        |
| 👶Inicial  | 0                | 0           | 0             | 0            |0            |>1 day      |

# How to use

To run this development you will need to have
1. wowlogs token (here's how to get it (link))
2. List of characters and alters UPDATED before run (based on GRM format (addon link))
3. CSV with manual inputs UPDATED before run(example in google sheets link)
4. CSV with bench attendance UPDATED before run(example in google sheets link)
5. Consumables files based on CLA inputs UPDATED before run (example in google sheets link)

# Output Example
| main character | good environment | good player | almost no lag | uses discord | consumables | attendance | rank     |
|----------------|------------------|-------------|---------------|--------------|-------------|------------|----------|
| Jmerrick       | 1                | 1           | 1             | 1            | 300         | 100%       | Exaltado |
| Aletss         | 1                | 1           | 1             | 1            | 260         | 70%        | Estable  |
| Littlewoman    | 0                | 1           | 1             | 1            | 200         | 45%        | 5050     |
| Pirru          | 1                | 0           | 0             | 1            | 120         | 15%        | Inicial  |
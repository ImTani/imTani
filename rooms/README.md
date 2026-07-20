# rooms/

A text adventure that lives in markdown. No Actions, no engine, no JavaScript —
each room is a file, each exit is a relative link. It works on GitHub, it works in
any editor, and it will still work in ten years.

## The map

```
                        ../README.md
                             |
                        [ the door ]
                             |
                          hall.md
             ________________|________________
            |         |          |            |
        lab.md   workshop.md  vault.md    archive.md
       (AiHello)   (clipd)  (SmoothSend)  (games, plugins)
                             |
                          study.md
                     (music, drawing, poems)
```

`study.md` is deliberately the one you have to go furthest to find.

## Writing a room

Copy `_template.md`. The only rules that matter:

1. **Second person, present tense.** "You are standing in..." not "This is..."
2. **One concrete object per room** the reader could pick up. Rooms without objects
   read like brochures.
3. **Exits last**, as a plain list of links. Never more than four.
4. **No explaining the joke.** If a room is about the repricer, don't say "this is
   about the repricer."

## Rules for yourself

- Every room is a real thing. No invented lore. The adventure is only interesting
  because it's true.
- Rooms may link to actual repos, files, songs, drawings. An exit that leaves the
  game is a good exit.
- Dead ends are fine. Not every room needs to go somewhere.

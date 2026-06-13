---
layout: default
---
# Uniform Musical Scale

Musical scales can be created

## Definition

**Building Blocks**

- Starting pitch class $P(0)$ (e.g. `C`)
- Musical interval $I$ in semitones (e.g. `P4 = 7 semitones`)

**Rules**

- From the start pitch, keep stepping by the selected interval. i.e. $P(n) = P(0) + n I$
- Stop when we loop back to the start. i.e.  $P(n) = P(0)$

## Scales, Enumerated

Since there are only 12 musical intervals, we can list all the possibilities

| Interval | Semitones | Scale starting on C | Notes (heh...) |
|---|---|---|---|
| Minor second (m2)        | 1  | `C C# D D# E F F# G G# A A# B` | C Chromatic scale |
| Major second (M2)        | 2  | `C D E F# G# A#` | C Whole Tone Scale |
| Minor third (m3)         | 3  | `C D# F# A` | Enharmonic to a C fully diminished chord |
| Major third (M3)         | 4  | `C E G#` | C augmented chord |
| Perfect fourth (P4)      | 5  | `C F A# D# G# C# F# B E A D G` | (Enharmonic to) Circle of Fourths |
| Tritone (T)              | 6  | `C F#` | Tritone interval |
| Perfect fifth (P5)       | 7  | `C G D A E B F# C# G# D# A# F` | Circle of Fifths, or Circle of Fourths descending |
| Minor sixth (m6)         | 8  | `C G# E` | C augmented chord, descending |
| Major sixth (M6)         | 9  | `C A F# D#` | C fully diminished chord, descending |
| Minor seventh (m7)       | 10 | `C A# G# F# E D` | C whole tone scale, descending |
| Major seventh (M7)       | 11 | `C B A# A G# G F# F E D# D C#` | C Chromatic scale,  descending |
| Perfect 8th (octave, P8) | 12 | `C` | C by itself |

## Other notes

🚧 Outline for now

- The table has a symmetry - `(invert_interval, reverse_scale)`
    - this is related to integers mod 12, e.g. `11 = -1` which is the additive inverse of `1`
- only two scales include all 12 notes
    - chromatic scale and circle of fourths
    - Group theory explanation - Lagrange theorem
    - Another explanation - 12 has a lot of divisors, but is coprime with 1 and 5 (as well as 7, 11)

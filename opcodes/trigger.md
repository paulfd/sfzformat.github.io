---
layout: "sfz/opcode"
lang: "en"
opcode_name: "trigger"
---
Values can be:

- ***attack*** : (Default): Region will play on note-on.
- ***release***: Region will play on note-off or sustain pedal off. The velocity
                used to play the note-off sample is the velocity value of the
                corresponding (previous) note-on message.
- ***first***: Region will play on note-on, but if there's no other note going on
                (staccato, or first note in a legato phrase).
- ***legato***: Region will play on note-on, but only if there's a note going on
                (notes after first note in a legato phrase).
- ***release_key***: SFZ v2 addition. Region will play on note-off.
                The velocity used to play the note-off sample is the velocity
                value of the corresponding
                (previous) note-on message. Ignores sustain pedal.

## Example

```
trigger=release
```

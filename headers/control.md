---
title: ‹control›
lang: en
---
SFZ 2 header can contain the following special directives, which should not
be used under other headers:

- [#define](/opcodes/define)
- [default_path](/opcodes/default_path)
- [note_offset](/opcodes/note_offset)
- [octave_offset](/opcodes/octave_offset)
- [label_ccN](/opcodes/label_ccN)
- [set_ccN](/opcodes/set_ccN)

Multiple <control> headers can be used in one file, in which case the older
<control> opcodes are replaced by the new <control> opcodes or reset to their
default. This can be very useful when specifying
[default_path](/opcodes/default_path). This path will then be used for all
regions until another <control> header is encountered.


See also [ARIA Extensions](/extensions/aria/#instrument-settings).

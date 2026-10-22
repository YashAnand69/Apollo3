# Apollo #867 graphical evidence

Native Chrome 155 / Cypress 16.2.0, local isolated collaboration server, identical GFF fixture and drag from CDS end 26 to 33. Display height enlarged only to show the full annotation table.

- Before: upstream helper at 106e48c92754b76c5992ec0c0cc7a2f46cef9b67. The CDS and mRNA end at 33; exon2 incorrectly remains at 28.
- After: reviewed utility-reuse fix. CDS, exon2 and mRNA end at 33; gene end remains 40.

Screenshots are unedited Cypress captures. Both evidence runs asserted these coordinates and passed. The committed regression separately checks Undo/Redo and persisted coordinates after reload.

Prepared with Codex assistance.

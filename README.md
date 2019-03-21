# Errorses
A library based on / with similar API to 'errors', except rather than building
an error off of a string, build an error object based on a slice of maps.

### API brainstorm
- Map: one error, including a string, maybe other attrs like debug level.
- Slice: ability to pass more than one error.
- Something like...
  - `func (self MultiErr) New (errs ...[]map[attrType]string) MultiErr {}`
  - or, `map[attrKeyType]attrValType`

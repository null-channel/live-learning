---

kanban-plugin: board

---

## TODO

- [ ] benchmark database really well
- [ ] [[Switch to byte offset]]
- [ ] remove main log lock
- [ ] Raft is not enough
- [ ] Snapshotting vs Compaction
- [ ] should pass in full roster, including self
- [ ] run in single node mode
- [ ] make a "run three quick" script?
- [ ] batch


## IN_PROGRESS

- [ ] Basic Raft [[NullDB/Consensus/Lesson Plan]]
- [ ] index is not incrementing
- [ ] Investigate performance issues
	1) build release, remove console logging
	2) update code to support single node.
	3) review multi-threading on client
	4) review multi-threading on server


## READY

- [ ] filesystem [[NullDB/FileSystem/Lesson Plan]]


## DONE





%% kanban:settings
```
{"kanban-plugin":"board","list-collapse":[false,false,false,false]}
```
%%
https://github.com/LMMS/lmms/pull/7477:

- MIDI clips
	- Cutting across a note with per-note automation can be done three ways:
		1. Don't cut
		2. Do a soft cut
		3. Do a hard cut, give both notes the same automation
			- This is a known issue: https://github.com/LMMS/lmms/issues/5940

- BB clips
	- Cutting BB clips is problematic because you can't tell where a cut has been made.
		- There are three ways to solve this:
			1. Don't implement BB cutting
			2. Add gray areas to BB clips (Not possible, BB clips are not unique, like MIDI clips are)
			3. Keep BB cutting as it is now, but add https://github.com/LMMS/lmms/pull/7559 so it's easier to comprehend

TODO:

- [ ] Address the issue of cutting across a pitch-bent note
- [ ] Address the issue of BB clip cutting ambiguity

---
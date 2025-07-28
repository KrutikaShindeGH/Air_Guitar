# Air_Guitar 🎸:
Control MIDI guitar strings in real-time using hand gestures captured from your webcam. Each finger is mapped to a chord in the D major scale, D_Dorian Scale, G_Mixolydian Scale, G_pentatonic Scale, phrygian Scale and strings play and sustain naturally as you move your fingers.

# How It Works 🧭:
- The webcam detects your hands in real-time using cvzone’s HandDetector.
- Each finger corresponds to a specific chord (left and right hands are mapped identically).
- When a finger is raised (fingersUp), a chord is played.
- When the finger is lowered, the chord sustains for a short delay before stopping.

# Chord Mapping (D Major Scale) 🎵:

| Finger | Chord (Notes) | Description |
|--------|---------------|-------------|
| Thumb	| D Major (62, 66, 69) | D - F# - A |
| Index | E Minor (64, 67, 71) | E - G - B |
| Middle | F# Minor (66, 69, 73) | F# - A - C# |
| Ring | G Major (67, 71, 74) | G - B - D |
| Pinky | A Major (69, 73, 76) | A - C# - E |

# Chord Mapping (D_Dorian Scale) 🎵:

| Finger | Chord (Notes) | Description |
|--------|---------------|-------------|
| Thumb | D Minor (62, 65, 69) | D – F – A |
| Index | E Minor (64, 67, 71) | E – G – B |
| Middle | F Major (65, 69, 72) | F – A – C |
| Ring | G Major (67, 71, 74) | G – B – D |
| Pinky | A Minor (69, 72, 76) | A – C – E |




# Chord Mapping (G_Mixolydian Scale) 🎵:

| Finger | Chord (Notes) | Description |
|--------|---------------|-------------|
| Thumb | G Major (55, 59, 62) | G – B – D |
| Index | A Minor (57, 60, 64) | A – C – E |
| Middle | B Diminished (59, 62, 65) | B – D – F |
| Ring | C Major (60, 64, 67) | C – E – G |
| Pinky | D Minor (62, 65, 69) | D – F – A |




# Chord Mapping (G_pentatonic Scale) 🎵:

| Finger | Chord (Notes) | Description |
|--------|---------------|-------------|
| Thumb | G Major (55, 59, 62) | G – B – D |
| Index | A Minor (57, 60, 64) | A – C – E |
| Middle | B Minor (59, 62, 66) | B – D – F♯ |
| Ring | D Major (62, 66, 69) | D – F♯ – A |
| Pinky | E Minor (64, 67, 71) | E – G – B |



# Chord Mapping (phrygian Scale) 🎵:

| Finger | Chord (Notes) | Description |
|--------|---------------|-------------|
| Thumb | E Minor (52, 55, 59) | E – G – B |
| Index | F Major (53, 57, 60) | F – A – C |
| Middle | G Major (55, 59, 62) | G – B – D |
| Ring | A Minor (57, 60, 64) | A – C – E |
| Pinky | B Diminished (59, 62, 65) | B – D – F |


# Code Overview 🔗
- pygame.midi.init() initializes MIDI output.
- cvzone.HandTrackingModule.HandDetector handles hand and finger tracking.
- fingersUp() determines which fingers are raised.
- MIDI notes are triggered with note_on and note_off functions.
- Chords are sustained for a configurable delay (SUSTAIN_TIME = 2.0).









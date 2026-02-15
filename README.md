# phonetics_scripts

A curated collection of Praat and Python scripts for phonetics research. These tools support acoustic analysis workflows including TextGrid annotation, duration extraction, and speech rhythm measurement.

## Scripts

### Modify_TextGrid.praat

Helper tool for efficient TextGrid annotation. Opens paired `.wav` and `.TextGrid` files sequentially, allowing you to edit and save annotations with a single button press.

**Features:**
- Batch processing of audio-TextGrid file pairs
- Supports same-directory or separate-directory layouts (e.g., `wavs/` and `textgrids/`)
- Press *Continue* to save and advance to the next file

**Usage in Praat:**
1. Open Praat
2. Run script: `Praat > Open Praat script... > Modify_TextGrid.praat`
3. Set the directory path(s) when prompted

### Extract_Duration.praat

Extracts segment durations from annotated TextGrid files. Outputs duration measurements for specified tiers and intervals.

**Usage in Praat:**
1. Open Praat
2. Run script: `Praat > Open Praat script... > Extract_Duration.praat`
3. Configure input directory and tier settings

### calculateRhythm.py

Python script for calculating speech rhythm metrics from duration data. Computes standard rhythm measures used in L2 speech research.

**Requirements:**
- Python 3.6+
- NumPy

**Usage:**
```bash
python calculateRhythm.py
```

## Related Publications

- Park, S. (2023). "Interpretation of speech rhythm: Speech error, speech rhythm, and speech proficiency." *JASA* 153(3_supplement), A343.
- Park, S. & Warner, N. (2023). "The role of probability and duration in perception of speech sounds." *Speech Communication* 152, 102950.

## Author

Seongjin Park — [seongjinpark.com](https://seongjinpark.com)

## License

MIT

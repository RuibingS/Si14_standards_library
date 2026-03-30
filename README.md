# Si14_stanards_library

## Description
LC-MS/MS spectral library of 14 pure reference standards measured as a mixture., converted from
Bruker `.library` format to NIST MSP format with spectral entropy annotation.
This library is an ongoing collection and will be updated as new compounds
are measured.

## Repository Contents

| File | Description |
|------|-------------|
| `library/Si14_library.msp` | Final NIST MSP library file |
| `library/Si14_library.library` | Original Bruker source file |
| `library/Si14_library_MS.library` | Original Bruker source file |
| `library/Si14_library_MS2.library` | Original Bruker source file |

## Instrument

- **Instrument:** Bruker maXis HD (QTOF)
- **Ionization:** ESI positive and negative mode
- **MS levels:** MS1 and MS2



## MSP Format

Each entry contains the following fields:

```
Name: Naproxen
Formula: C14H14O3
ExactMass: 230.09429430766
Ion_mode: POSITIVE
Spectrum_type: MS1
Instrument_type: ESI-TOF
Instrument: maXis HD
Ionization_method: ESI
Collision_energy: 7
RetentionTime: 750.693
Spectral_entropy: 2.796424
Quality: CLEAN
Comments: Contributor=CBIO
Num Peaks: 124
115.0541 0.7007
128.062 0.2002
141.0698 0.7007
142.0773 0.4004
144.0332 0.1001
147.5524 0.1001
152.0619 0.6006
153.0697 1.001
154.0772 0.8008
155.0849 0.3003
155.5413 0.5005
158.0726 1.4014
...
```

## Spectral Entropy

Spectral entropy is calculated as described in:

> Li, Y. et al. Spectral entropy outperforms MS/MS dot product similarity
> for small-molecule compound identification. *Nature Methods*, 2021.
> <https://doi.org/10.1038/s41592-021-01331-z>

Quality flags assigned per entry:

| Flag | Meaning |
|------|---------|
| `CLEAN` | Reliable spectrum — entropy above quality threshold |
| `NOISY` | Low entropy — use with caution |

## License

CC0 1.0 Universal — Public Domain.
You are free to use, share, and build upon this data without restriction.
Attribution is not legally required but is appreciated — please cite the
associated publication if you use this library in your work.

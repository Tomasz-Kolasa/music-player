# Music Player

A simple **Python audio player application** developed as part of university laboratory exercises.

The project focuses on practicing Python programming, object-oriented programming and implementing an algorithm for generating unique shuffled playlists.

## Overview

The application allows the user to create a playlist from a collection of available music albums and shuffle the songs in the playlist.

One of the main requirements of the project was that each generated shuffle should produce a **unique song order**.

The project uses a collection of albums represented as nested Python tuples and lists.

## Features

* Create a playlist from available songs
* Shuffle songs in the playlist
* Generate a unique song order for each shuffle
* Keep track of previously generated song orders
* Organize music data using Python collections
* Separate application logic into classes

## Shuffle Algorithm

A key requirement of the project was:

> Every generated shuffled song order must be unique.

Two possible approaches were considered:

1. Generate a random song order when requested and remember previously generated orders.
2. Generate all possible permutations in advance and provide them one at a time.

The first approach was selected for this project.

When a new shuffle is requested, a random order is generated and compared with previously generated orders to ensure that the same arrangement is not returned again.

This approach is simple and practical for the scope of the project, while avoiding the potentially large memory requirements of generating all possible permutations in advance.

## Project Structure

```text
music-player/
├── albums/
│   └── Music data
├── classes/
│   └── Application classes
├── player.py
└── README.md
```

## Technologies

* **Python**
* **Object-oriented programming**
* **Lists and tuples**
* **Randomization**
* **Algorithmic problem solving**

## Purpose

This project was developed as part of university laboratory exercises.

Its main purpose was to practice:

* Python programming
* object-oriented programming
* working with collections
* designing simple application logic
* implementing and evaluating different algorithmic approaches
* handling requirements and their trade-offs

The application should therefore be considered an **educational project rather than a production-ready music player**.

## Design Considerations

The requirement to generate unique shuffled orders introduces a trade-off between simplicity and memory usage.

Generating all possible permutations beforehand could require a significant amount of memory as the number of songs increases.

The implemented approach generates permutations on demand and stores previously generated orders. This keeps the implementation simpler and avoids calculating the entire permutation space upfront.

## Disclaimer

This project is a university programming exercise and is not intended to represent a complete commercial audio player.

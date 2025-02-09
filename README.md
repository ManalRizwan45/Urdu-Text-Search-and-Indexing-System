# Urdu Text Search and Indexing System

## Overview
This project implements an **inverted index** for an **Urdu text corpus**, enabling efficient text indexing and retrieval. It processes a document collection, excludes stop words, creates an index of terms, and stores positional data for quick and accurate search queries.

## Features
- **Indexing Mechanism:** Generates a structured term list with document frequency and linked postings.
- **Stop Word Removal:** Filters out common words to enhance search efficiency.
- **Positional Indexing:** Records exact locations of terms within documents.
- **Optimized Storage:** Utilizes linked lists for scalable indexing.
- **Search and Retrieval:** Allows users to input terms and fetch document IDs with positional information.

## File Structure
- `invert.py` - Reads the Urdu corpus, builds the inverted index, and writes index and postings files.
- `test.py` - Reads indexed files and retrieves document IDs and positions for user-input terms.
- `index.txt` - Stores the sorted term list with document frequency.
- `postings.txt` - Contains postings for each term, sorted by document and position.

## Setup & Execution
1. **Install Dependencies:**
   ```sh
   pip install nltk
   ```
2. **Run the Indexing Program:**
   ```sh
   python invert.py
   ```
3. **Run the Search Program:**
   ```sh
   python test.py
   ```
4. **Input Search Terms:** Enter a word to retrieve its occurrences in the corpus.

## License
This project is open-source and available under the MIT License.


# 🏥 Healthcare CDC (Change Data Capture) Pipeline

## Problem Statement

Healthcare systems frequently update patient and claims data. Traditional batch pipelines introduce delays. This project simulates a CDC-based pipeline to process incremental updates in near real-time.

## Architecture

* Initial Load: Patient dataset ingested
* Incremental Updates: New and updated records captured
* Merge Logic: Handles inserts and updates
* Output: Final dataset reflecting latest state

## Tech Stack

* Python
* Pandas
* Simulated Streaming (CDC concept)

## Data Flow

1. Load initial dataset
2. Stream incremental updates
3. Apply merge logic (upsert)
4. Generate updated dataset

## Key Features

* Simulates CDC (Change Data Capture)
* Handles inserts & updates
* Demonstrates incremental processing
* Reduces dependency on full batch loads

## Use Cases

* Patient record updates
* Claims processing systems
* Real-time healthcare analytics

## How to Run

1. Add datasets in `/data`
2. Run:
   python src/process_updates.py
3. Check output in `/output/final_data.csv`

## Outcome

* Reduced latency compared to batch processing
* Efficient incremental data handling
* Real-world CDC pipeline simulation

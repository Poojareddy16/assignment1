**Assignment 1 – Docker Compose Stack**

This project demonstrates a basic multi-container setup using Docker Compose. It includes:

A Postgres database that is automatically seeded with sample trip data.

A Python application that connects to the database, runs SQL queries, and produces a summary of the trips.

The application prints the summary to the logs and also saves the same data into the out/summary.json file. This makes it easy to both view results directly and keep them stored locally.

Outputs

Logs: Show the summary JSON when the app runs.

File: A copy of the results is written to out/summary.json.

Notes

The Python app is designed to run once, produce results, and then exit successfully (exit code 0).

The database container remains running until stopped.

If the database is not ready when the app starts, simply re-run the stack.

Ensure the out/ folder exists and has write permissions before starting.


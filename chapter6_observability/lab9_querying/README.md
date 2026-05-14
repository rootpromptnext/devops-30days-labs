# Lab 9: Log Querying

## Objective
Query logs using LogQL.

## Prerequisites
- Loki installed

## Steps
1. Run LogQL queries.
2. Filter by labels.

## Commands
```logql
{job="nginx"} |= "error"

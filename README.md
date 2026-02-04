Working with larger-than-RAM data using duckdbfs

## Overview

This module explores high-performance workflows for tabular data using `duckdbfs` to work with datasets larger than available RAM by leveraging DuckDB's streaming and remote file access capabilities.

## Case Study: Global Supply Chains

We work with [EXIOBASE 3.8.1](https://source.coop/youssef-harby/exiobase-3), a global Multi-Regional Input-Output (MRIO) database that tracks economic transactions between sectors and regions, along with their environmental impacts.

**Data Specifications:**
- **Coverage**: 44 countries + 5 rest-of-world regions
- **Timeframe**: 1995–2022
- **Content**: Economic transactions (Z matrix), final demand (Y matrix), and environmental stressors (F matrix)
- **Format**: Cloud-optimized Parquet, partitioned by year and matrix type
- **Source**: [EXIOBASE 3 on Source Cooperative](https://source.coop/youssef-harby/exiobase-3)

## Files

- `tabular-data.qmd`: Main analysis notebook with exercises on remote data access, filtering, and aggregation

## Requirements

- R with the following packages:
  - `duckdbfs`
  - `dplyr`

## Topics Covered

1. Connecting to remote cloud-based datasets without downloading
2. Efficient filtering and querying of large datasets
3. Aggregating and analyzing environmental impact data
4. Working with partitioned Parquet files

## Course

ESPM 288 - Data Science for Environmental Management

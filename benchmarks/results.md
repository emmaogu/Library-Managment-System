# Performance results

### Find one book by ISBN (time per lookup)

| Books | Hash table | Linear search |
|---|---|---|
| 1,000 | 0.68 µs | 100.34 µs |
| 10,000 | 3.18 µs | 1,542.12 µs |
| 100,000 | 3.90 µs | 57,246.45 µs |
| 1,000,000 | 2.07 µs | 124,288.03 µs |

### Sort all books

| Books | Merge sort | Bubble sort |
|---|---|---|
| 100 | 0.61 ms | 1.35 ms |
| 1,000 | 9.09 ms | 204.20 ms |
| 5,000 | 35.00 ms | 5,627.43 ms |
| 10,000 | 113.39 ms | not run (too slow) |
| 100,000 | 2,343.51 ms | not run (too slow) |
| 1,000,000 | 15,917.40 ms | not run (too slow) |

### Find one book by title in a sorted list (time per search)

| Books | Binary search | Linear search |
|---|---|---|
| 1,000 | 8.41 µs | 66.35 µs |
| 10,000 | 11.03 µs | 1,219.68 µs |
| 100,000 | 11.78 µs | 15,764.83 µs |
| 1,000,000 | 11.83 µs | 94,474.01 µs |

### Add then serve every reservation

| Reservations | Linked-list queue | Python list pop(0) |
|---|---|---|
| 1,000 | 1.96 ms | 0.33 ms |
| 10,000 | 12.83 ms | 17.51 ms |
| 100,000 | 117.87 ms | 2,069.37 ms |

### Add loans then remove them in due-date order

| Loans | Min-heap | Sorted Python list |
|---|---|---|
| 1,000 | 9.58 ms | 1.96 ms |
| 10,000 | 155.49 ms | 60.89 ms |
| 100,000 | 1,886.58 ms | 4,935.12 ms |

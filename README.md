# Data is growing rapidly
![](assets/data-growth.png)
# Opportunity: Data duplication is common
## Sources of duplicate data
- The same files are stored by multiple users into the cloud
- Continuously updating of files to generate multiple versions
- Use of check pointing and repeated data archiving
## Significant data duplications has been restored
- For backup storage workload
    - Over 90% are duplicate
- For primary storage workload
    - About 50% are duplicate
# The duplication technique help
![](assets/simple-dedupe.png)
# Deduplicate at smaller chunks
![](assets/chunking-and-fingureprint.png)    
# Fixed size chunking
![](assets/fixed-size-chunking.png)
Boundary shift problem
![](assets/boundary-shift-problem.png)
# Content defined chunking
![](assets/content-defined-chunking.png)
# Parallelizing CDC Chunking Operations
![](assets/cdc-parallelization.png)
Following is details on compromised deduplication ratio
![](assets/cdc-parallel-dedupe-compromised.png)
Chunks can be different 
![](assets/cdc-parallel-problem.png)
# Goal of algo
To design a parallel chunking technique with following goal
- does not compromise y deduplication ratio
- achieves super linear speedup of chunking operations
# SS-CDC Chunking
![](assets/ss-cdc-phase-1.png)
![](assets/ss-cdc-phase-2.png) 
# Advantage SS-CDC Chunking
![](assets/ss-cdc-advantage.png)
# Single thread/core chunking throughput
![](assets/ss-cdc-result1.png)
# Multi thread chunking throughput
![](assets/ss-cdc-result-2.png)
# Existing Parallel CDC deduplication ratio reduction
![](assets/regular-cdc-result-1.png)
# Reference
https://www.youtube.com/watch?v=NqzoDpO6W2w

https://blog.gopheracademy.com/advent-2018/split-data-with-cdc/

https://restic.net/blog/2015-09-12/restic-foundation1-cdc

https://www.bertil.ch/pubs/W5L3JRBE.pdf


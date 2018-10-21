# Memory Report  

515110910011  李晗东  

## Vendors or types or technologies  

### Top eight memory card market vendors

SanDisk  

Kingston Technology  

Lexar (Micron Consumer Products Group)  

ADATA Technology  

Transcend Information  

Samsung Group  

Sony  

Toshiba  


### types of memory  

Synchronous Dynamic RAM (SDRAM)  
Single Data Rate Synchronous Dynamic RAM (SDR SDRAM)  
Double Data Rate Synchronous Dynamic RAM (DDR SDRAM, DDR2, DDR3, DDR4)  
Graphics Double Data Rate Synchronous Dynamic RAM (GDDR SDRAM, GDDR2, GDDR3, GDDR4, GDDR5)  

Now most of personal computers use DDR3 or DDR4(or their low-voltage version) as main memory, and some computers use GDDR4 or GDDR5 in thier GPU.  

### Emerging Memories  

3D Xpoint  
MRAM


### Features  

### Pros&Cons  

Pros  
  
High speed  
Temporary memory (volatile)  
Faster than secondary storage  
Fastest type of memory in a computer.  
Consumes less power compared to disk drives hence increasing battery life.  

Cons  

Slower than the CPU cache  
Not cost friendly  
Volatile  
Space limited  

## Key indicators  

1. CAS Latency  

CAS Latency (Column Access Strobe Latency), or tCL, specifies the number of clock cycles between the column strobe signal and when data is available on the output pins. During sequential memory accesses, the row remains activated and only the column changes, which means that the time required to change columns is critical to overall memory performance. CAS Latency, often abbreviated CL, is the most commonly quoted timing parameter and the most important memory timing parameter with respect to overall performance.

2. RAS to CAS Delay  

RAS to CAS Delay (Row Access Strobe to CAS Delay), or tRCD, specifies the number of clock cycles between the time a row is activated by the row strobe until the column in that row (which defines a memory cell or bit) can be read or written. When memory is accessed sequentially, the row is already active and only the column changes, so tRCD has little impact on performance. But when memory is accessed randomly, the memory controller must deactivate the old row and activate a new row, which incurs a substantial timing penalty. In that situation, a fast tRCD contributes to faster memory performance.

3. RAS Precharge Delay  

RAS Precharge Delay, or tRP, specifies the time required to complete one row access, deactivate that row, reactivate the next row, and begin the next row access. The time required to switch rows and select the next memory cell is therefore the sum of tRP and tRCD. For sequential memory accesses, a slow tRP has little effect; for random memory accesses, a fast tRP contributes significantly to overall memory performance.

4. Precharge Delay

Precharge Delay, or tRAS, specifies the number of clock cycles between the time a row is accessed (activated) and when data can be read from that row. Once the row is activated, data can be read from that row without further overhead until the end of the row is reached, so tRAS ordinarily has little effect on overall memory performance. As with any timing parameter, setting tRAS incorrectly can reduce system stability.

These four memory timing parameters are always listed in the order given, separated by hyphens. For example, a particular PC3200 DDR-SDRAM module may list timings of 2-2-2-5, which means that module is designed to operate with timings of two clock cycles for CAS, tRCD, and tRP, and five clock cycles for tRAS. Similarly, a PC2-3200 DDR2-SDRAM module might list timings of 5-5-5-12, which means that module is designed to operate with timings of 5 clock cycles for CAS, tRCD, and tRP, and 12 clock cycles for tRAS. (Note that DDR and DDR2 timings are not directly comparable, because DDR2 operates on much shorter clock cycles.)


###  How to measure performance

we can use software like AIAD64

## My comment  

1. Memory provides a fast way to swap data in CPU and disks, so if possible choosing a memory with bigger volume and faster speed always helps. 

2. We can use multiply memories to form double channel to speed up system.  

3. The speed gap between CPU cache and memory is still large.

4. If the cost of memory drops, it's a good idea to use memory as disk, but we need to take care of power-off.


### Reference 

1. https://www.cnet.com/how-to/test-your-ram-with-windows-memory-diagnostic-tool/

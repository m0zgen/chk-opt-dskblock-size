## Checking optimal block dd size

Usage
```bash
bash check.sh /mnt/ssd-data/t/test_file   
```

Output:
```bash
Generating test file...
block size : transfer rate
     512 : 567 MB/s
    1024 : 1.0 GB/s
    2048 : 2.1 GB/s
    4096 : 2.0 GB/s
    8192 : 3.7 GB/s
   16384 : 4.3 GB/s
   32768 : 2.9 GB/s
   65536 : 4.1 GB/s
  131072 : 4.1 GB/s
  262144 : 3.3 GB/s
  524288 : 4.6 GB/s
 1048576 : 3.0 GB/s
 2097152 : 2.7 GB/s
 4194304 : 3.0 GB/s
 8388608 : 2.7 GB/s
16777216 : 2.5 GB/s
33554432 : 2.9 GB/s
67108864 : 1.7 GB/s
```

Winner:
```
524288 : 4.6 GB/s
```

Reference:
* https://stackoverflow.com/questions/6161823/dd-how-to-calculate-optimal-blocksize/27772496

## Given-a-list-slice-it-into-a-3-equal-chunks-and-rever-each-list
## Sample code to check for 3 equal chunks
```sh
sampleList = [11, 45, 8, 23, 14, 12, 78, 45, 89]
print("Original list ", sampleList)

length = len(sampleList)
chunkSize  = int(length/3)
start = 0
end = chunkSize
for i in range(1, 4, 1):
  indexes = slice(start, end, 1)
  listChunk = sampleList[indexes]
  print("Chunk ", i , listChunk)
  print("After reversing it ", list(reversed(listChunk)))
  start = end
 ```
 ## Expected output
 Original list  [11, 45, 8, 23, 14, 12, 78, 45, 89]
Chunk  1 [11, 45, 8]
After reversing it  [8, 45, 11]
Chunk  2 [23, 14, 12]
After reversing it  [12, 14, 23]
Chunk  3 [78, 45, 89]
After reversing it  [89, 45, 78]

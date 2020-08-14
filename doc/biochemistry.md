# Gene Expression

## Handling reads

### Different terms

There are a number of terms that are used in the subject of reads mapped to genes:

1. **FPKM: Fragments per kilobase million**
   1. **Adapted for**: paired-end RNA seq
   2. Because in paired-end RNA seq there are two main conditions:
      1. both reads of the pair map to a single fragment
      2. one read of the pair maps to a single fragment and the other does not. 
   3. FPKM takes into account that two reads *can* map to a single fragment. 
2. **RPKM: Reads per kilobase million**
   1. **Adapted for**: single-end RNA seq
3. **TPM: Transcripts per million**
   1. Similar to the other two
   2. **Difference**: the order of operations
      1. $\frac{\text{Read counts}}{\text{Gene len in kb}}$, do this for every gene? This gives reads per kilobase (RPK)
      2. $\frac{\text{All counted RPK in sample}}{1\times 10^6} = C$ , this is per million scaling factor
      3. $C \times \begin{bmatrix}RPK_1\\ \vdots \\ RPK_N\end{bmatrix}$

#### TPM

In effact the 

### RPKM

Short for: Reads per Kilobase per million (mapped reads). 
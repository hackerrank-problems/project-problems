You are given `n` tasks, each with a difficulty level represented by the array `difficulty[i]`, where `1 ≤ i ≤ n`. A task `j` (where `1 ≤ j ≤ n`) is considered valid if there exists a task `i` (where `1 ≤ i < j`) such that:

- **If `i` and `j` have the same parity**:
  \[
  \text{difficulty}[i] + \text{difficulty}[i+2] + \dots + \text{difficulty}[j] = \text{difficulty}[i+1] + \text{difficulty}[i+3] + \dots + \text{difficulty}[j-1]
  \]

- **If `i` and `j` have different parity**:
  \[
  \text{difficulty}[i] + \text{difficulty}[i+2] + \dots + \text{difficulty}[j-1] = \text{difficulty}[i+1] + \text{difficulty}[i+3] + \dots + \text{difficulty}[j]
  \]

Find the smallest index `j` that qualifies as a valid task. Use 1-based indexing. If no valid task exists, return `-1`.
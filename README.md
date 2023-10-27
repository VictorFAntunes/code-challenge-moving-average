## Coding Interview Question: Iterator-based Moving Average of the Largest 5 Numbers

​

### Problem Statement

​

Your task is to implement a function in Scala that computes the moving average of the largest 5 numbers from a given series of numbers. The function should accept an `Iterator[Double]` and return an `Iterator[Option[Double]]`.

​

Each element in the output iterator should represent the moving average of the largest 5 numbers in the sequence up to that point. If fewer than 5 numbers have been processed, the output should yield `None`.

​

### Requirements

​

- **Language**: Standard Library Scala.

- **Input**:It should accept an iterator over numbers (`Iterator[Double]``) as its only argument.

- **Output**: A new iterator (`Iterator[Option[Double]]`)

- **Constraints**: If fewer than 5 numbers have been processed, the iterator should yield None.

- **Important**: Should be implemented efficiently to handle large series



### Function Signature

​

Function signature to be implemented:

​

```

def movingAverageOfTop5(input: Iterator[Double]): Iterator[Option[Double]]

```

​

### Example

​

Assume inputIterator is an iterator over the list [10, 20, 30, 40, 50, 25, 35].

​

When you call movingAverageOfTop5(inputIterator), the returned iterator should yield the following sequence:

​

```

List(None, None, None, None, Some(30.0), Some(33.0), Some(36.0))

```

​

### Tips

​

- Think about how you can maintain the state efficiently while iterating.

- Consider using functional programming paradigms like `foldLeft` for your implementation.

​

### Extra-challenge:

- Show an implementation using an Fs2 Streams 

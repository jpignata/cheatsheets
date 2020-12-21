# Comprehensions

## Flatten a list

```python
[number for group in [[1, 2], [3, 4]] for number in group]

=> [1, 2, 3, 4]
```

# Matrices

```python
grid = [[1, 2, 3, 4],
        [5, 6, 7, 8]]
```

## Flip horizontally

```python
[row[::-1] for row in grid]

=> [[4, 3, 2, 1], [8, 7, 6, 5]]
```

## Flip vertically

```python
grid[::-1]

=> [[5, 6, 7, 8], [1, 2, 3, 4]]
```

## Rotate 90 degrees (clockwise)

```python
[list(row) for row in zip(*grid[::-1])]

=> [[5, 1], [6, 2], [7, 3], [8, 4]]
```


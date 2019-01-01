# py-readability-metrics

Score text difficulty usings a variety of _readability_ metrics including: Flesch-Kincaid Grade Level, Flesch Reading Ease, and more

## Install

```shell
pip install py-readability-metrics
```

## Usage

```python
from readability import Readability

 r = Readability(text)
 print(r.flesch_kincaid())
 print(r.flesch())
 print(r.gunning_fog())
```

### Flesch-Kincaid Grade Level

**method:**

```python
r.flesch_kincaid()
```

**returns:**

```python
Result(
    score, # float
    grade_level # string
)
```

### Flesch Reading Ease

**method:**

```python
r.flesch()
```

**returns:**

```python
Result(
    score, # float
    ease, # string
    grade_levels, # list<str>
)
```

### Gunning Fog

**method:**

```python
r.gunning_fog()
```

**returns:**

```python
Result(
    score, # float
    grade_level, # str
)
```

## Contributing

[see contributing](CONTRIBUTING.md)

## License

[MIT](LICENSE)

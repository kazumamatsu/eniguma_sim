# enigma_simulater

## Overview

This is 3 rotors enigma simulater
３ローターのエニグマシミュレータです。  

## Quickstart

### Installation
```python
python -m pip install git+https://github.com/kazumamatsu/enigma_sim.git
```

### Using enigma_simulater in a Python script
1. Import module
```python
import enigma
```

1. Setting config
```python
config = list("AAA")
```
1. Encryption
```python
E = enigma.enigma(config[0], config[1], config[2])
text = list(str.upper("AAA"))
print(text)
code = []
for t in text:
  code.append(E.typing(t))
  E.print(ptype = 0)
print(code)
```

1. Decoding
```python
E = enigma.enigma(config[0], config[1], config[2])
decode = []
for t in code:
  decode.append(E.typing(t))
  E.print(ptype = 0)
decode
```

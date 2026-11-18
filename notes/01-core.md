# Parse hexadecimal bytes: implementation

## What the example does

bytes.fromhex accepts ASCII whitespace between byte pairs. An odd number of digits or an invalid hex character raises ValueError.

The public function is `solve(value)`. The JSON input contract can be seen in this concrete example:

```json
"00 ff 10"
```

Expected result:

```json
[
  0,
  255,
  16
]
```

Run `python3 example.py` for the Python representation of the result. `solution.py` contains the full implementation and can also be imported by another script.

## Scope

The function implements exactly the behavior described above. It does not perform network or filesystem access. Python exceptions indicate unsupported input; the next lesson turns them into a command-line error response. Review the limitations before reusing it in an application.

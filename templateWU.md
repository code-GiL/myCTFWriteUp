# [Challenge Title]

> **Platform:** 
> **Category:** Web Exploitation / Cryptography
> **Points:** 100
> **Difficulty:** Easy / Medium / Hard

## Challenge Description
> *Paste the challenge description here for context.*
> "Can you find the secret cookie hidden in this website?"

**Link/File:** [Link to challenge or file]

## Reconnaissance / Analysis
Explain your initial steps. What did you check first?

1. I accessed the website and inspected the source code (`Ctrl+U`).
2. I noticed a suspicious cookie named `auth`.
3. The cookie value looked like Base64 encoding: `YWRtaW4=`

## Exploitation / Solution
Detail the technical steps taken to get the flag.

**Step 1: Decoding the Cookie**
I attempted to decode the value using the terminal:
```bash
echo "YWRtaW4=" | base64 -d
# Output: admin
```

**Step 2: Modifying the Value Since the cookie value was admin**
I tried modifying it to...
(Insert screenshot if necessary)

## Solver Script (Optional)
If you wrote a script to automate the solution, include it here.
```python
import requests
# Script ...
```

## Flag
CTF{this_is_an_example_flag}

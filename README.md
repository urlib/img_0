# A repo for delivering binary files

```text
ALGO: SHA256
SALT: ec39fb41547dc9878dccfae96e69fc9e4269841e7cb1d54757680d25369a71db
```

```python
def run_sha_256(url: str, content: bytes) -> str:
    sha = hashlib.sha256(SALT.encode())
    sha.update(url.encode())
    sha.update(content)
    return sha.hexdigest()
```

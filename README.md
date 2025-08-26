# Importing Public Key

To verify signatures, you will need my public key in your keyring. You can import it from GitHub or a public key server.

- Import directly from GitHub (recommended for simplicity):
  ```bash
  curl -sL https://github.com/falmontejb.gpg | gpg --import -
  ```

- Import from a public key server (fingerprint-based retrieval):
  ```bash
  gpg --keyserver hkps://keys.openpgp.org --recv-keys 27E90E80866C1535B3892FCEF996E8396C86372A
  ```

After importing, verify the key is present:
```bash
gpg --list-keys 27E90E80866C1535B3892FCEF996E8396C86372A
```


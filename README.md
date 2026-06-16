# ket4kids.com

Password-gated static site. Client-side AES-GCM (PBKDF2-SHA256, 250k iter).

`content.html` and `build.py` are gitignored — they live on the maintainer's machine only. The repo only contains the encrypted artifact and the page shell.

## Rebuild after editing content

```
PASSWORD=<the-password> python3 build.py
git add index.html && git commit -m "update" && git push
```

GitHub Pages auto-deploys from `main`.

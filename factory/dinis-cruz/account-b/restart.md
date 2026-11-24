# Restart notes

What a fresh perspace.b session needs to know.

- Committed here: role, decisions, messages, learnings, open work, the public key.
- Not committed, by design: the private research, the vault working copy, the vault key, the read key and perspace.b's private keys. They lived only in the old session's private scratch space.
- If the old session is gone: the vault key is held by b.maestro; the read link and QR code are held by Dinis. The served zip in site/private/ is the sealed copy of the site.
- A fresh session makes its own new key (sgit pki keygen --label perspace.b@SovereignWebsite.dinis), publishes the public half here in a commit of its own, and asks for the old key to be retired in team/keys.json.
- To change the sealed site, the fresh session needs the vault key from b.maestro through a signed decision request.

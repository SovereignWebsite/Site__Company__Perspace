# Learnings

- The environment sets a global git signing program that signs with the machine key. In this repository, set gpg.ssh.program to ssh-keygen and user.signingkey to your own key, then check each commit with an allowed_signers file before pushing.
- html-validate 8.24.0 rejects --preset=standard; the gate template's --config works.
- A gated site gets no start, agents or admin pages, no agents.json, no llms.txt. Only the holding page, open.js and the ciphertext zip are served.
- Sending a sealed key to another session can be stopped by the session's own permission check. Report only what was actually delivered, and correct at once if a report ran ahead.
- A key holder that cannot open the key file can prove possession with a SHA-256 of the key value; compare it, never the key.
- Never put a proof value, key or token in a message, a request or this area.

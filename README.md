# iusmaris.com — Preview (password-protected)

This is the **preview version** of the Ius Maris Climaticum website, sitting behind a soft password gate so the convenors and invitees can review the programme before public launch.

## Password

The inscription reads *"Speak, friend, and enter."* The gate accepts any of:

```
friendship
friend
mellon
```

(Case-insensitive.) The intended password to share with invitees is **friendship**. The other two are quiet concessions to anyone who recognises the riddle and answers it directly — "friend" being the English answer, "mellon" the Sindarin original on the Doors of Durin.

## How the gate works

`index.html` is the password page. On correct entry, it sets a `localStorage` flag (`imc-preview-access = granted`) and redirects to `home.html` (the actual landing page). All four content pages (`home.html`, `programme.html`, `participants.html`, `practical.html`) check that flag at the top of the document and redirect back to the gate if it's missing.

The gate is **client-side only** — the password string lives in `index.html`'s `<script>` block. It's a soft barrier, suitable for an invitation-only preview. It is not, and is not intended to be, cryptographic protection.

## When the workshop is ready to go public

Replace the contents of the GitHub repository with the contents of the sibling `05_Website/` folder (which has no gate and no auth checks). That will be the public launch state.

## Structure

```
.
├── index.html         The password gate
├── home.html          Home page (formerly index.html in the public site)
├── programme.html
├── participants.html
├── practical.html
├── style.css
├── assets/
├── CNAME              Custom domain for GitHub Pages
└── README.md
```

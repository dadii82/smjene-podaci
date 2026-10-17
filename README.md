# smjene-podaci

Šifrirani raspored za aplikaciju „Smjene i vrtić”. `plan.enc` je JSON omot oko
podataka zaključanih lozinkom (PBKDF2-SHA512 → XSalsa20-Poly1305, tweetnacl
`secretbox`). Bez lozinke je sadržaj nečitljiv.

Datoteku piše isključivo poslužitelj na djdevu; mobiteli je odavde samo čitaju
kad djdev nije dostupan.

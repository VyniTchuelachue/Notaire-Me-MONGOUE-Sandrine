# smnotaire.com — Étude de Me Sandrine MONGOUE

A static, bilingual (FR/EN) website for Me Sandrine MONGOUE, notary holding the 9th office of Douala (Akwa).
No build step, no database, no server code: upload the files and it works.

```
index.html          French home page (main language)
en/index.html       English version
assets/css/site.css shared styles
assets/js/site.js   mobile menu, document checklists, WhatsApp / e-mail message builder
assets/img/favicon.svg
robots.txt, sitemap.xml
```

## Deploying to smnotaire.com

The domain already points to a host showing a default "Votre site est opérationnel" page.

1. Log in to the hosting panel (cPanel / file manager) or connect by FTP.
2. Open the web root (usually `public_html/` or `www/`) and remove or rename the host's placeholder `index.html`.
3. Upload everything in this folder **except** `README.md` and the `.claude/` folder, keeping the structure.
4. Enable HTTPS (free Let's Encrypt certificate in most panels).
5. Check `https://smnotaire.com/` and `https://smnotaire.com/en/`.

The contact form and the checklists don't need a mail server. They open the visitor's WhatsApp or e-mail app with a pre-written message to +237 690 97 80 98 / sandrine.mongoue@smnotaire.com.

## Content sources

Every fact about the office comes from:
- the prospecting sheet (address, phones, e-mail, clients from Google reviews),
- the Chambre nationale des notaires list (2019): 9th office of Douala, date 23 June 2017, B.P. 5374, holder of the records of Maître MBOBDA MONGOUE Elie,
- the Google Maps listing (plus code 2MXV+2GP).

The pages contain no invented biography, testimonials, ratings or opening hours.

## To confirm with Me MONGOUE before going live

- [ ] **WhatsApp:** is 690 97 80 98 on WhatsApp, and should clients use it?
- [ ] **English:** can the office answer messages in English? (The EN page implies it can.)
- [ ] **Payment advice:** she agrees with the note "confirm bank details by calling the landline before paying".
- [ ] **Document lists** (Pièces à fournir): she reviews and adjusts each list, especially company formation and marriage contracts.
- [ ] **Remote process:** the "sign before a notary abroad or legalise at the consulate" wording matches how she handles procurations.
- [ ] **Opening hours:** add them to the contact section if she wants them shown.
- [ ] **Photo:** a portrait or a photo of the office would strengthen "L'étude" (none is used now).
- [ ] **Seal design:** the violet "SM" stamp is a decorative proposal, not her official seal.

## Previewing locally

Open `index.html` directly in a browser, or serve the folder with any static server
(for example `npx serve .`) to test the `/en/` links.

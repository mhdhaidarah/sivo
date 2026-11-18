<p align="center">
  <img src="sivo-logo.svg" width="112" alt="SIVO logo">
</p>

<h1 align="center">SIVO</h1>
<p align="center"><b>SecuryTik IPTV &amp; Video Operations</b><br>
Your own IPTV service, served from a server inside your network.</p>

<p align="center">
  <a href="https://sivo.securytik.com">Website</a> ·
  <a href="https://sivo.securytik.com/docs">Docs</a> ·
  <a href="https://sivo.securytik.com/pricing">Pricing</a> ·
  <a href="https://sivo.securytik.com/terms">Terms and Policy</a> ·
  <a href="https://github.com/mhdhaidarah/sivo/releases/latest">Latest release</a>
</p>

---

## Why SIVO

An internet provider that sells TV pays for the same channel once per viewer on its uplink. SIVO pulls each live
channel **once** and serves every subscriber from a server inside the provider's own network, so a thousand
viewers cost the uplink of one. Subscribers keep the apps they already use.

| | |
|---|---|
| 📺 **Live TV** | Each channel pulled once and restreamed (HLS) to every viewer; started when someone watches, stopped a minute after the last one. A backup source per channel; a branded no-signal screen while a source is down. |
| 📡 **Video inputs** | Restream TV from boxes in your own network: multicast from IP encoders and satellite or cable receivers (each channel of a multi-channel feed picked on its own), encoders and cameras over SRT, RTSP, RTMP, HTTP or UDP, HDHomeRun tuners and Tvheadend servers. Add the box, SIVO scans it, tick the channels to import. |
| 🎬 **Movies & series** | A library on your own disks: posters, stories, cast, seasons and episodes, several audio tracks and subtitles per title. |
| ⏪ **Catch-up & TV guide** | Record chosen channels for 1 to 30 days; XMLTV guides matched to channels. |
| 📱 **Every IPTV app** | Xtream Codes API and M3U for IPTV Smarters, TiviMate, VLC and smart-TV apps — no app of ours needed. |
| 👥 **Subscribers & packages** | App login, expiry with date and time, devices at once; packages open live categories, all movies and all series. |
| 💳 **Billing** | Invoices (full or segmented), down payments, wallets, cash accounts, agents, cashier, reports, profit and loss; online payments with Stripe, PayPal, Binance Pay, Sham Cash and Whish Money. |
| 🌐 **Subscriber portal** | Subscribers sign in with their app login to renew, change package, pay online and read their invoices. |
| 🛡️ **Admins & roles** | Branches, roles with detailed permissions, two-factor login, audit log, backups, signed updates. |
| 🔌 **API** | REST API with scoped tokens for subscribers, packages, content, invoices, payments and collection apps; signed webhooks. |
| 🗣️ **Eight languages** | English, Arabic, Turkish, French, Spanish, German, Russian and Persian. |

## Install

On a fresh **Ubuntu 24.04 or 26.04 server (x86_64)** inside your network, as root:

```bash
curl -fsSL https://sivo.securytik.com/install.sh | sudo bash
```

**github.com blocked in your country?** The command above detects it and switches to the SecuryTik mirror by
itself — or install straight from the mirror:

```bash
curl -fsSL https://dl.securytik.com/sivo-install.sh | sudo bash
```

Then open `http://<server-ip>/admin/` and sign in as `admin` with the password the installer prints. Set the address
your subscribers' apps use in **Settings → Streaming**, add channels, create a package and your first subscriber.

## Plans

Counted by subscribers only — channels, movies, series and devices are never limited.

| Plan | Subscribers | Price |
|---|---|---|
| Free | 100 | Free |
| Lite | 500 | 25 USD / month |
| Plus | 1,000 | 35 USD / month |
| Pro | 2,000 | 50 USD / month |
| Mega | 5,000 | 75 USD / month |
| Max | 10,000 | 100 USD / month |
| Unlimited | ∞ | 175 USD / month |

Yearly billing gets two months free. Register the server from **System → License** with your SecuryTik account.

## Content is yours

SIVO is **software only**. SecuryTik sells no channels, streams, playlists or servers. The only content shipped is an
optional starter list of free channels that each broadcaster streams itself. Everything else you add — channels,
M3U lists, provider accounts, movies and series — is your responsibility: hold the rights and licences for it in every
country where you offer it. Read the [Terms and Policy](https://sivo.securytik.com/terms).

## Updates

SIVO checks for signed releases daily and updates itself from **System → Update**.

---

© SecuryTik, Beirut, Lebanon — [securytik.com](https://securytik.com) · [sivo@securytik.com](mailto:sivo@securytik.com)

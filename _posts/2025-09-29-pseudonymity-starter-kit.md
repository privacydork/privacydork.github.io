---
layout: post
title: Pseudonymity Starter Kit - what to buy, how to configure it, and how to use it safely
---

You want to exist online under a name that doesn't map to your passport, employer, or landlord. Good. That's doable, but it's not a product you can buy and forget. It's a posture you assemble: identities, network hygiene, hardened accounts, and payment rails, combined and maintained. Below are the concrete tools I recommend, why they matter, and the exact toggles and habits I'd use to get them from zero to a functioning pseudonymous persona.

# The short list (starter kit - get these if you want one-stop readiness)

- Password manager ([Bitwarden](https://bitwarden.com/), [1Password](https://1password.com))
- Hardware security key ([Yubikey](https://www.yubico.com/), [Nitrokey](https://www.nitrokey.com/), [SoloKey](https://solokeys.com))
- [Tor Browser](https://www.torproject.org/download/) (official build) for sensitive browsing
- Audited VPN ([Mullvad](https://mullvad.net/en), [Proton](https://protonvpn.com)) for everyday IP-reduction; prefer audited, RAM-only servers
- One E2EE messenger for content ([Signal](https://signal.org/)) and one username-first option ([Matrix/Emement](https://element.io/) or [Session](https://getsession.org/)) depending on threat model
- A cheap secondary device (used laptop or burner phone) or VM to separate stacks
- A small cash reserve and a plan for low-trace payments (prepaid cards, legal entity if you expect imcome)

# Set up, step-by-step

## 1. Identity stacks - build three, now

Create: **public/legal**, **pseudonymous**, **operational (throwaway)**. Write them down on paper and never link them together online.

Do this immediately:

- Create a **new email** for your pseudonymo (pick a provider you control - a paid account helps avoid spam and weird auto-flagging). Don't use your mail Gmail. Use [Proton](https://proton.me/mail) or [TutaNota](https://tuta.com/).
- In your password manager, create a **folder** for that pseudonym and put every username and password there. [Bitwarden](https://bitwarden.com/) supports folders and orgs for this.
- Pick a plausible persona (age range, city, profession) and stick to it. Plausibility is camouflage.

Why: separation limits blast radius. If the pseudonym burns, your legal life doesn't.

## 2. Browser & device isolation - do this next

Minimum viable isolation:

- Use **separate browser profiles**: one for public/legal, one for pseudonymous. Disable cross-profile sync.
- For higher safety, use a second physical device or a VM for your pseudonymous work. If you have the skill, [Qubes](https://www.qubes-os.org/)-style compartmentalization is idea; otherwise separate devices + strict habits are far better than nothing

Tor vs VPN:

- Use **Tor Browser** for high-sensitivity browsing (research, sources) - use the official Tor Browser and don't install extensions. Tor is overt and slow, but strong for IP avoidance.
- Use an **audited VPN** (Mullvad, Proton) for everyday pseudonymous browsing to reduce direct IP linage while keeping UX sane. Prefer providers that run RAM-only servers and publish audits.

Practical toggle: when creating the pseudonym account, register and do light browsing witht he VPN, then use Tor for truly sensitive steps. Don't mix sessions.

## 3. Messaging - pick two, configure them

Pick one primary messenger for content confidentiality and one for username-first or numberless identity.

- **Signal** - content encryption is excellent; enable **Registration Lock**, **Screen Lock**, and **Disappearing Messages** for sensitive threads. Signal is phone-number based; that's convenient but also a linking vector. Use Signal when you can accept the phone-number model.
- **Matrix/Element** - great if you want username-based accounts and optional self-hosting. Element now supports robust end-to-end encryption and voice/video for self-hosted users. If you self-host a homeserver, you control one of the trust points - but keep in mind federation metadata.
- **Session** - build to avoid phone numbers by design and uses onion-style routing; a good choice when you want numberless identity (but check current maturity/audit status).

Config checklist:

- Turn on registration lock or equivalent
- Enable disappearing messages for sensitive groups
- Verify safety numbers/fingerprints when talking to key contacts

## 4. Accounts & authentication - make account takeover hard

- Use a password manager (Bitwarden) and create unique, long passwords for every login. Put pseudonym credentials in a separate folder.
- Buy a **hardware security key** (Yubikey, Nitrokey, Solokey). Register a dedicated key for your pseudonym's critical accounts (email for that identity, your password manager entry for that identity). Keep one backup key in a secure place.
- Do **not** register the same hardware key on both your public and pseudonymous stacks if you care about total orthoganality - a shared key is an easy pivot. Ifyou must, understand the linking risk.

## 5. Payments - pragmatic options

- For small purchases: cash and prepaid cards are simplest.
- For creator income: consider an **LLC** (talk to an accountant, find your regional equivalent). It creates legal separation but requires proper tax reporting.
- If you dig crypto: learn [CoinJoin](https://www.coinjoins.org/) and privacy best practices or Monero fundamentals - but treat these as advanced and regulatory-fragile options; exchanges require KYC for fiat on/off ramps and my delist privacy coins.

# Quick test & verification routine (do this monthly)

1. Log into each stack from its intended environment (public from public device/profile, pseudonym from its device/profile). Ensure no cross-login cookies.
1. Check Bitwarden folders: no public credentials in pseudonym folder.
1. Confirm hardware key registration is correct and a backup key exists.
1. Run a Tor Browser session and a VPN session; confirm each hides your IP the way you expect (use known IP-check sites only). Rotate servers occasionally for VPN.

# Pitfalls you absolutely must avoid

- Don't reuse recovery email or phone numbers across stacks - that's the single most common rookie mistake.
- Don't post the same image across identities. Reverse-image search will link you fast.
- Don't register your pseudonym account on the day you register your public account form the same IP. Stagger creation timings. Playsibility matters.
- Don't rely on E2EE alone - metadata (who you message, when) leaks. Design your behavior accordingly

# Quick reference: where each tool wins

- [Signal](https://signal.org/) - content confidentiality, great UX; phone-number tether.
- [Matrix/Emement](https://element.io/) - username-first, federated, self-hostable. Good for pseudonyms.
- [Session](https://getsession.org/) - numberless messaging via onion-style routing; good for hiding the phone link.
- [Tor Browser](https://www.torproject.org/download/) - best ofr single-session IP unlinkability; use for sensitive research.
- [Mullvad](https://mullvad.net/en), [Proton](https://protonvpn.com) VPNs - audited, privacy-respecting VPNs with RAM-only servers/audits - practical everyday IP reduction.
- [Bitwarden](https://bitwarden.com/)) - vault folders for per-stack separation - offline password maanger.
- [Yubikey](https://www.yubico.com/), [Nitrokey](https://www.nitrokey.com/), [SoloKey](https://solokeys.com) - FIDO2 hardware keys to stop account takeover.

# If you're an activist or journalist in a hostile place

This kit gives you a durable posture, but local reality matters. Do this instead of improvising:

- Coordinate with local or international NGOs for tested local guidance.
- Prefer collective, public adoption of privacy tools where possible (it reduces individual targeting).
- Prioritize low-tech fallbacks and legal preparation.

# One-page quickstart checklist

- Create 3 identity stacks (public/pseudonymous/operational)
- New email + Bitwarden folder for pseudonym
- Second device or VM for pseudonym
- Install Tor Browser; subscribe to an audited VPN
- Pick messaging: Signal + Matrix/Session (configure registration lock, disappearing messages)
- Purchase a hardware key; register it for pseudonym-critical accounts
- Build cash/prepaid fallback; consult tax/corporate counsel if you'll earn money ynder a pseudonym

# Final note - this is ongoing work

Pseydonymity is not a one-and-done install. Tools change, audits happen, providers are compelled by courts, and your own habits can betray you. Treat this kit as a living posture: pick the right adversary, adopt the minimum that defends you against them, and keep the plan updated.

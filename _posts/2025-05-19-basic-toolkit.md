---
layout: post
title: Anonymous Internet Access 101
---

This guide is written for people who don't have a strong technical background, and may live in places where the internet is more locked down than a vault. Carefully following these instructions should have even the least technical people up and running with anonymous access to the open internet with the most convenience possible.

## Understand the Risks

Before jumping into the world of uncensored browsing:

- Assess the risks: Be aware of the potential legal, social, or personal consequences in your region. If you're in the USA or most of Europe, it is perfectly legal and acceptable to access the internet in the ways described in this post. However, if for instance you're a whistleblower, you may still endure some kind of consequence for your actions if you're caught. If you live in regions that heavily censor the internet like China or Iran, you may need to be mindful of other consequences if you're caught.
- Keep it low-key: Avoid drawing attention to your activities, especially in areas where using tools to circumvent internet censorship can attract unwanted attention.

## Choosing a Tool

When it comes to acessing the free internet, there are several tools at your disposal. I'll talk about them in more detail below, but to help you skip to a section that might make the most sense for you, here's a quick breakdown of the pros and cons to each of the tools this post covers.

| Tool | Best For | Pros | Cons |
| ---- | -------- | ---- | ---- |
| Tor Browser | Anonymity and browsing the open web | Best for anonymous browsing. Free, open-source, and widely used. The default option for everyone. | Often blocked in highly censored regions (but possible to make work without too much trouble). Slower speeds due to encryption and anonymization techniques makes it unsuitable for watching videos. |
| VPNs (Virtual Private Networks) | Hiding your location and bypassing censorship | Easy to use. Provices extra security on top of Tor, or independently. | Some countries block VPNs. Less anonymous than Tor, the VPN provider can still track your activity if not configured properly. |
| Lantern | Circumventing heavy censorship | Simple to use and effective in highly restricted areas like China. Lightweight and doesn't require a technical background. | less anonymous than Tor. Limited security compared to other options. |

## Setting up Tor

Tor is the default option for anyone looking to participate anonymously on the internet. Tor Browser is a special web browser that has Tor built into it, and it's what most people should be using. It's easy to install and get running, as you'll see here. **Tor works by encrypting and routing your data through at least three different computers in three different countries, making it essentially impossible to track you. This collection of different computers is called the Tor Network.**

If you live in a place where the government allows you to use Tor, you can and should download it from the official Tor website, [torproject.org](https://www.torproject.org/download/). It is very important to download Tor from the official site if you are able, to avoid inadvertently installing a version that someone malicious has tampered with. Tor Browser is available on Windows, macOS, Linux, and Android. iOS has an option called Onion Browser, which is *not* Tor Browser, but does route your traffic through the Tor network.

## What if Tor's blocked?

In some countries, Tor's website might be blocked entirely. But don't worry, you're not out of luck. Here are way sto get Tor when the website is blocked.

### GetTor - Download Tor via Email or Telegram, Alternative Downloads

- **Email**: Send an email to [**gettor@torproject.org**](mailto:gettor@torproject.org) with the subject line "windows", "macos", or "linux" (based on your operating system). You'll receive a response with links to download Tor hosted on a platform that is available in your country.
- **Telegram**: Message [**@GetTor_Bot**](https://t.me/GetTor_Bot) on Telegram. Type `/start` and select your operating system. The bot will give you the program so you can install it.

If the official Tor website is blocked, and you can't get it via email or Telegram, you can try these two mirrors which make Tor available for download.

- Calyx Institute: [calyx-institute.org](https://calyx-institute.org)
- Electronic Frontier Foundation (EFF): [eff.org/tor](https://www.eff.org/tor)

### Accessing the Tor Network

If the official Tor website is blocked in your country, they are probably also trying to prevent you from accessing the Tor network in general. Luckily, there are a number of options to help get you connected online anonymously.

#### Bridges - A Backdoor into Tor

What they are: Bridges are private entry points into the Tor network. They're harder to block and provide an alternative way to connect when Tor's usual paths are closed off.

- Requesting Bridges - different options
  - If you have access to the Tor website, you can get them at [bridges.tornetwork.org](https://bridges.torproject.org/options)
  - Send an email to [**bridges@torproject.org**](mailto:bridges@torproject.org) *from a Gmail or RiseUp account* with the subject line `get transport obfs4`

Tor will send you bridge addresses you can use to connect. In the Tor Browser, when you click `Configure`, select `I need a bridge` and input the bridge addresses you received.

#### Snowflake - Volunteer Proxies to the Rescue

What it is: Snowflake is another tool that lets you connect to Tor by routing your traffic through volunteer-run proxies.

- How to use Snowflake:
  - In Tor Browser: Go to `Configure` > `I need a bridge` > Choose `Snowflake`
  - Snowflake will help you bypass censorship and connect to Tor automatically

- In Orbot (for Android): Go to `Settings` > Enable Snowflake under the Bridges section

## VPNs

A VPN is like a cloak that hides your internet activity and makes it appear as if you're browsing from another location. Great for masking your IP and bypassing local restrictions.

- Recommended VPNs:
  - [ProtonVPN](https://protonvpn.com/): Strong privacy policies, free and paid versions.
  - [Windscribe](https://windscribe.com/): Free tier with limited data and servers.

- How to use:
  - Install the VPN app on your device.
  - Connect to a server in a country where the internet isn't censored.
  - Once connected, you can download Tor, or simply browse the internet freely.

##  Lantern - The Censorship Bypass Tool

Lantern is a free and open-source tool designed to help you bypass censorship, especially in countries where even VPNs are blocked.

- How to use Lantern:
  - Download Lantern from [Lantern.io](https://lantern.io).
  - Install and open the app. it will automatically connect you to the internet without censorship.

Lantern is not as widely used or support when compared to Tor. Lantern is a good tool and worth trying if you can't make Tor Browser work.

## Secure Communication

For private communication, you'll want to use secure tools:

- Email: Use services like [ProtonMail](https://protonmail.com) or [TutaNota](https://mail.tutanota.com/) to send and receive messages.
- Secure Messaging: Use apps like [Signal](https://signal.org/#signal) or [Threema](https://threema.com/en/products/private) for encrypted messaging to protect your conversations.

## Stay Informed and Safe

- Keep Tools Updated: Always update Tor, your VPN, and other tools to stay protected from new security risks.
- Stay Anonymous: Don't share personal information that oculd connect you to your activities online.
- Stay Low-Key: Be mindful of your online presence. Not everone needs to know you're using Tor or other circumvention tools.

## Important Notes

- Legal Stuff: In some countries, using tools like Tor or VPNs can be illegal or monitored. Always be aware of the risks in your region. You alone are responsible for your activities, this information is provided to educate and without guarantees or liability.
- Safety First: Your safety is the top priority. Use these tools responsibly and securely.

## Additional Resources

- [Tor Browser User Manual](https:tb-manual.torproject.org)
- [Tor Bridges Documentation](https://tb-manual.torproject.org/bridges)
- [Snowflake Information](https://snowflake.torproject.org)

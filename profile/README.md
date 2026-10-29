## Yundera: a managed private server with open-source apps, ready from day 1.

As self-hosters, we were tired of spending time fixing broken updates, applying manual fixes and dealing with unexpected regressions. Ask yourself:

- That Immich or Nextcloud instance you set up: when did you last update it?
- Those Docker containers running critical services: are they still on last year's versions?
- That backup system you configured: when did you last check that it actually restores?
- Those SSL certificates you set up by hand: are they about to expire?

Self-hosting gives freedom, but maintenance quietly becomes a burden. So we built an open-source Private Cloud Server stack that makes self-hosting reliable and accessible, in two layers:

- **NSL.SH (MeshRouter)**: a free, MIT-licensed layer that brings any server or NAS online in one click. Every app gets its own subdomain (`app-you.nsl.sh`) with HTTPS, even behind CGNAT, with no port to open and no DNS to configure. It ships with **Maison**, our dashboard and app manager, an App Store of curated apps whose configurations are reviewed and kept up to date, single sign-on with 2FA in front of every app, and nightly self-updates. [nsl.sh](https://nsl.sh) · [mesh-router-root](https://github.com/Yundera/mesh-router-root)
- **Yundera**: the same open stack on a server we provide and maintain for you. Think of it as a virtual NAS, available in one click: apps kept up to date by our team and by developers in the Yundera Creator Program, backups included, nothing to run at home. [yundera.com](https://yundera.com)

If you already self-host, Yundera lets you forget about broken updates, manual fixes and regressions. If you are new to it, Yundera is a safe starting point: install apps knowing they are maintained, without configuring a domain or learning server administration.

---

## How the stack fits together

| Layer | What it does | Repository |
| --- | --- | --- |
| Routing | Free subdomains, HTTPS, tunnel through CGNAT | [mesh-router-root](https://github.com/Yundera/mesh-router-root) |
| Box template | Installs and self-updates everything below | [mesh-router-template-root](https://github.com/Yundera/mesh-router-template-root) |
| Sign-in | Single sign-on (Dex + Authelia) with 2FA, one login for every app | [mesh-router-template-root](https://github.com/Yundera/mesh-router-template-root) |
| Dashboard | Maison: home screen, App Store, backups, domains, resource history | [Maison](https://github.com/Yundera/Maison) |
| Files | Web file manager | [files](https://github.com/Yundera/files) |
| Apps | Curated App Store | [AppStore](https://github.com/Yundera/AppStore) |

It helps you:

- Install open-source apps with confidence: one click, no domain to configure
- Avoid updates that break your setup
- Run services on infrastructure you control
- Keep predictable costs and full ownership of your data

No lock-in. No hidden SaaS dependencies. Open source, running on your own infrastructure.

---

## What you will find in this organization

- Core infrastructure components
- Networking and routing tools
- App templates and integrations
- Utilities for self-hosting and automation
- Documentation and examples

Each repository is focused, modular and designed to be reusable.

---

## Contributing

- Join our Creator Program: [yundera.com/creator-program](https://yundera.com/creator-program)
- Report bugs on our Discord: [discord.gg/f2qQUJBHY6](https://discord.gg/f2qQUJBHY6)
- Submit pull requests
- Review app configurations
- Share feedback from real usage, with us or with your friends

---

## Documentation and resources

- Blog and tutorials: [yundera.com/blog/tutorial-1](https://yundera.com/blog/tutorial-1)
- Community: [Discord](https://discord.gg/f2qQUJBHY6)
- Documentation: [docusaurus-yunderateam.nsl.sh](https://docusaurus-yunderateam.nsl.sh)
- Tech News Digest: [ghost-yunderalabs.nsl.sh](https://ghost-yunderalabs.nsl.sh)

---

## Our philosophy

- Self-hosting should be accessible, not reserved for experts
- Open-source tools are powerful when they are easy to use
- Owning your infrastructure means owning your freedom

Yundera exists to lower the barrier between people and their own servers.

Thanks for stopping by. If you like self-hosting, you are in the right place 🙂

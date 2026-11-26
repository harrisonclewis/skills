# ai-skills

A collection of agent skills for building production web apps, from API design and authentication to testing, hardening and shipping with AI agents.

## Install

```bash
npx skills add harrisonclewis/skills
```

Or as a Claude Code plugin:

```bash
/plugin marketplace add harrisonclewis/skills
/plugin install ai-skills@ai-skills
```

## Skills for building the backend

- [**api**](skills/api/SKILL.md): Designs and reviews HTTP JSON APIs and their persistence, from **request flow**, **response and error shape** and **status codes** to **pagination**, **transactions**, **migrations**, **seeders** and **audit events**.
- [**auth**](skills/auth/SKILL.md): Builds account flows that never reveal whether an account exists, covering **sign-up**, **sign-in and MFA**, **password and email changes**, **invitations**, **deletion** and **sessions**, tested byte for byte.
- [**security**](skills/security/SKILL.md): Applies the security rules every line of code follows, from **sessions**, **CSRF**, **headers and CSP** and **authorisation** to **API keys**, **emailed codes**, **redirects** and **logging**.
- [**ops**](skills/ops/SKILL.md): Takes an app from working to safe and operable with **rate limits**, **CAPTCHA**, **observability**, **alerting**, the **admin console**, **privacy and compliance**, **email delivery**, **deployment** and **incident response**.
- [**naming**](skills/naming/SKILL.md): Sets one naming vocabulary across **routes**, **handlers**, **pages**, **client calls**, **permissions**, **events** and **rate limits**, based on Laravel resource actions.

## Skills for building the frontend

- [**frontend**](skills/frontend/SKILL.md): Builds the web frontend in any framework, covering **routing**, **data loading**, **mutations**, **paginated lists**, **forms**, the **design system** with **typography**, **colour**, **layout**, **surfaces** and **motion**, **UX copy**, **accessibility** and **seeing every state** before it ships.

## Skills for keeping a codebase healthy

- [**structure**](skills/structure/SKILL.md): Decides **where code goes** and **what may import what**, from the route registry and handler layers to frontend folders and test placement.
- [**testing**](skills/testing/SKILL.md): Sets what is worth testing and how, from **integration tests on a real database** and **endpoint coverage** to **permission matrices**, **race tests**, **frontend unit tests** and **e2e**.
- [**tooling**](skills/tooling/SKILL.md): Builds the local loop and CI around **one command surface**, with **Docker Compose**, **env files**, **guarded test databases**, **parallel e2e** and **operator commands**.
- [**conventions**](skills/conventions/SKILL.md): Keeps conventions true over time with **checks written as tests**, a **docs folder**, **plans and recorded decisions**, **rename discipline** and **agent etiquette**.

## Skills for shipping with agents

- [**delivery**](skills/delivery/SKILL.md): Takes a feature from **raw notes** to a **merged commit** through plans, a build loop with **blind security review**, **overnight runs**, **parallel worktrees** and the **agent roles**.

## License

[MIT](LICENSE)

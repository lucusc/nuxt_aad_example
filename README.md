# nuxt_aad_example

Experimenting with NUXT and Authorization Code Flow with PKCE

## Getting started

Strongly suggest using VS Code and utilize Dev Containers.

```bash
git clone https://github.com/lucusc/nuxt_aad_example.git
cd nuxt_aad_example
code .
```

Once VS Code opens it should prompt you to re-open in develoment container. do that.

### env variables

Duplicate .env.sample and setup your settings

```bash
cp .env.sample .env
```

Add in your Azure AD Tenant Id and Client ID for your app registration.

### Debugging

Not fully working. Seems there are some issues with NUXT and the webpack source maps. Still trying to figure it out. Breakpoints are Unbound in VS Code until I figure this out.

Start debugging by hitting **F5**

This will start a debugging session for the NUXT Server side and Client Side.

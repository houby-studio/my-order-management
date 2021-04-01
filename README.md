# My Order Management - MOM

Direct evolution of [Small Business Fridge](https://github.com/houby-studio/small-business-fridge).  
Separate backend in C# and frontend in Quasar (Vue.js), communicating via REST API, CI/CD, dockerized, logging, monitoring and with mobile application.

# Preparing environment

## Links

- https://code.visualstudio.com/docs/containers/quickstart-aspnet-core
- https://code.visualstudio.com/docs/remote/containers-tutorial
- https://code.visualstudio.com/docs/containers/docker-compose
- https://next.quasar.dev/quasar-cli/installation

## Tasks

- Install VSCode
- Install Docker Desktop
- Install Yarn
- Install Visual Studio 2019
- Run VSCode
- Run Docker Desktop
- Install extension ms-vscode-remote.remote-containers
- Install extension ms-dotnettools.csharp
- Install quasar cli - command below
- Create new frontend project - command below (only during creation)
- // Create new backend projects - command below (only during creation)
- Install Visual Studio 2019
- Currently, there is one backend project created in Visual Studio 2019
  - Template: Web Application ASP.NET Core
  - Web API ASP.NET Core 5.0
  - Configured for HTTPS
  - Docker support
  - OS Linux
  - Enable OpenAPI support
  - Authentication for Work or school account, single organization, read directory data
- In VSCode run command:
  - Docker: Add Docker Files to Workspace... 
  - .NET: ASP.NET Core
  - Linux
  - 80,443
  - Yes
- Hit F5 and browse https://localhost:55000/swagger/index.html to view backend API

## Code

```powershell
# Setup frontend
yarn global add @quasar/cli
# Once Quasar V2 is out of beta, drop the branch parameter
quasar create mom-frontend --branch next
# Enable ESLint, TypeScript, Vuex, Axios, Vue-i18n
# Select Composition API
# Use Standard preset
# Use Yarn

# TODO: Setup backend with dotnet CLI
# MOM.Basket
# MOM.Catalog
# MOM.Identity
# MOM.Ordering
# MOM.Payment
# MOM.Webhooks
```

# Technologies to consider

- fluentd - logging for docker
- envoy - docker proxy
- prometheus - docker monitoring
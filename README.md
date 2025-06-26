# Code samples for Microsoft identity platform documentation - .NET, C\#

Welcome to the Microsoft Identity Platform .NET Code Samples repository!

This repository provides a comprehensive set of end-to-end samples demonstrating how to integrate Microsoft Entra ID authentication and authorization into .NET applications. The samples are organized by scenario and technology, making it easy to find the right starting point for your needs.

## 📁 Repository Structure

The samples are grouped into five main categories, each corresponding to a common application scenario:

│ ├── 1-server-side/ # Web APIs, Daemon apps, Blazor Server, ASP.NET Core ├── 2-client-side/ # SPA apps (Angular, React, Vue, Blazor WASM) ├── 3-desktop/ # WinForms, WPF, WinUI, Console ├── 4-migration/ # Migration guides (e.g., ADFS to Microsoft Entra) ├── 5-advanced/ # Advanced scenarios (e.g., distributed token cache) └── README.md

Each scenario folder contains one or more samples, each with its own README and instructions.

---

## 🗂️ Sample Scenarios

| Folder                                 | Description                                                                                  |
|----------------------------------------|----------------------------------------------------------------------------------------------|
| **[1-server-side](./1-server-side/)**  | Server-side web apps and APIs using ASP.NET Core, Blazor Server, and daemon/background apps. |
| **[2-client-side](./2-client-side/)**  | Single-page applications (SPA) using Blazor WASM, Angular, React, or Vue.                    |
| **[3-desktop](./3-desktop/)**          | Desktop applications using WinForms, WPF, WinUI, or Console.                                 |
| **[4-migration](./4-migration/)**      | Migration playbooks and samples (e.g., ADFS to Microsoft Entra).                             |
| **[5-advanced](./5-advanced/)**        | Advanced scenarios such as distributed token cache, multi-tenant, and custom policies.       |

---

## 🚀 Getting Started

1. **Browse the scenario folders** above to find the sample that matches your use case.
2. **Read the sample’s README.md** for prerequisites, setup instructions, and code walkthroughs.
3. **Clone and run the sample** following the provided steps.

All samples are built with the latest supported .NET versions and Microsoft.Identity libraries.

---

## 🔍 Finding the Right Sample

- **By scenario:** Start with the folder that matches your application type (server-side, client-side, desktop, migration, advanced).
- **By technology:** Within each folder, samples are organized by technology (e.g., ASP.NET Core, WPF, WinForms).
- **By feature:** Each sample README highlights the authentication flow, APIs called, and any advanced features.

---

## 📝 Configuration & Security

- **Configuration** is managed via `appsettings.json` and environment variables.
- **Secrets and credentials** should never be committed to source control. Use [Azure Key Vault](https://learn.microsoft.com/azure/key-vault/general/basic-concepts) or environment variables for sensitive data.
- **PowerShell scripts** are provided where helpful for Microsoft Entra app registration.

---

## 🤝 Contributing

We welcome contributions!  
Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on submitting new samples or improvements.

---

## 📢 Support & Feedback

- For questions, open an [issue](https://github.com/your-org/ms-identity-docs-code-dotnet/issues).
- For Microsoft identity platform documentation, visit [learn.microsoft.com/entra/identity-platform](https://learn.microsoft.com/entra/identity-platform).

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

Happy coding!

## Contents

| Sample directory                                    | Application type | Feature(s) demonstrated | Authentication libraries used |
|:----------------------------------------------------|------------------|-------------------------|-------------------------------|
| [console-cli](./console-cli)                        |                  |                         |                               |
| [console-daemon](./console-daemon)                  |                  |                         |                               |
| [desktop-winforms](./desktop-winforms/)             |                  |                         |                               |
| [desktop-winui](./desktop-winui/)                   |                  |                         |                               |
| [desktop-wpf](./desktop-wpf/)                       |                  |                         |                               |
| [spa-blazor-wasm](./spa-blazor-wasm/)               |                  |                         |                               |
| [web-api](./web-api/)                               |                  |                         |                               |
| [web-api-azure-function](./web-api-azure-function/) |                  |                         |                               |
| [web-api-obo-client](./web-api-obo-client/)         |                  |                         |                               |
| [web-api-obo-user](./web-api-obo-user/)             |                  |                         |                               |
| [web-app-aspnet](./web-app-aspnet/)                 |                  |                         |                               |
| [web-app-blazor-server](./web-app-blazor-server/)   |                  |                         |                               |
| [xplat-maui](./xplat-maui/)                         |                  |                         |                               |

## Resources

- Documentation on learn.microsoft.com
  - [Microsoft identity platform product documentation](https://learn.microsoft.com/entra/identity-platform/)
  - [Microsoft Authentication Library (MSAL) documentation](https://learn.microsoft.com/entra/identity-platform/msal-overview)
- Authentication library source code on GitHub
  - [Microsoft Authentication Library for .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
  - [Microsoft.Identity.Web](https://github.com/AzureAD/microsoft-identity-web)

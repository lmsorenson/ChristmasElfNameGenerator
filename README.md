# Christmas Elf Name Generator

This repository contains a **Blazor WebAssembly** app that generates random elf names. It's designed to deploy as a static site to Azure Static Web Apps (or any static hosting).

## Run Locally

```bash
cd src/ChristmasElfNameGenerator.Client
dotnet run
```

Open the URL reported by `dotnet run` (typically https://localhost:5001).

## GitHub Actions Workflow

The `.github/workflows/azure-static-web-apps-thankful-stone-0d7286710.yml` workflow:
1. Sets up .NET 8
2. Runs `dotnet publish -c Release -o publish_output`
3. Uploads `publish_output/wwwroot` to Azure Static Web Apps

The workflow is configured to find `index.html` in the `publish_output/wwwroot` directory.

## Project Structure

- `src/ChristmasElfNameGenerator.Client/` — Blazor WebAssembly project
  - `Pages/Index.razor` — Main elf-name generator UI
  - `Shared/MainLayout.razor`, `NavMenu.razor` — Layout components
  - `wwwroot/index.html` — Entry point (static)
  - `wwwroot/css/app.css` — Styles
# ChristmasElfNameGenerator
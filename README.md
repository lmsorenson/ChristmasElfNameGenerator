# Christmas Elf Name Generator

This repository now contains a minimal Blazor WebAssembly app scaffold under `src/ChristmasElfNameGenerator.Client`.

Run the WebAssembly app locally:

```bash
cd src/ChristmasElfNameGenerator.Client
dotnet run
```

By default the app will report the URL(s) to browse (for example `https://localhost:5001`).

What I added:

- A Blazor WebAssembly project at `src/ChristmasElfNameGenerator.Client` (`.csproj`, `Program.cs`).
- A simple UI (`Pages/Index.razor`) that generates a random elf name.
- Shared layout and basic CSS under `Shared/` and `wwwroot/css/app.css`.

If you previously relied on a static `index.html` in `wwwroot` for CI/CD, this WebAssembly project includes `wwwroot/index.html` so your workflow should find a default file.

Next steps I can do for you (pick one):

- Create a solution file and VS Code launch/tasks.
- Add a small CI workflow that runs `dotnet publish` and uploads the `publish/wwwroot` artifacts.
- Convert to a hosted (server + client) Blazor model.

Which of the above would you like next?
# ChristmasElfNameGenerator
# Welcome to My Profile! 👋 
![https://github.com/CyberTKR](https://img.shields.io/badge/Github-CyberTKR-black)
![https://instagram.com/_aquariusman](https://img.shields.io/badge/Instagram-__aquariusman-purple) ![Profile views](https://gpvc.arturio.dev/quiec)
![https://youtube.com/CyberTK](https://img.shields.io/badge/https://youtube.com/-CyberTK-red)



 ‏‏‎ ‎|  ‏‏‎ 
 --- | ---
**My Computer**  | `İmac, Windows"`
**Editor**  | `Visual Studio Code, Atom, Pycharms`
**Platforms I develop for** | `Desktop, Mobile, Web, CLI`
**Languages I know**  | `Python, JS, HTML`
**Languages I learning** | `Go, C#, C++, Swift, Ruby`


 ‏‏‎ ‎|  ‏‏‎ 
 --- | ---
![Metrics](https://metrics.lecoq.io/CyberTKR?template=classic&config.timezone=Europe%2FIstanbul&config.animated=true) | ![spotify-github-profile](/img/example.svg)

<img src="https://opencollective.com/armeria/contributors.svg?width=890&button=false" alt="Contributors">

# Visit https://github.com/lowlighter/metrics/blob/master/action.yml for full reference
name: Metrics
on:
  # Schedule updates (each hour)
  schedule: [{cron: "0 * * * *"}]
  # Lines below let you run workflow manually and on each commit
  push: {branches: ["master", "main"]}
  workflow_dispatch:
jobs:
  github-metrics:
    runs-on: ubuntu-latest
    steps:
      - uses: lowlighter/metrics@latest
        with:
          # Your GitHub token
          token: ${{ secrets.METRICS_TOKEN }}
          # GITHUB_TOKEN is a special auto-generated token restricted to current repository, which is used to push files in it
          committer_token: ${{ secrets.GITHUB_TOKEN }}

          # Options
          user: CyberTKR
          template: terminal
          base: header, activity, community, repositories, metadata
          config_timezone: Europe/Berlin


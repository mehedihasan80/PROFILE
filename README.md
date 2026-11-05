# PROFILE
<p align="center">
  <img src="https://github.com/YOUR_USERNAME/YOUR_USERNAME/blob/master/github-metrics.svg" alt="Metrics">
</p>
name: Metrics
on:
  schedule: [{cron: "0 0 * * *"}] # প্রতিদিন একবার আপডেট হবে
  workflow_dispatch:
  push: {branches: ["master", "main"]}

jobs:
  github-metrics:
    runs-on: ubuntu-latest
    permissions:
      contents: write
    steps:
      - uses: lowlighter/metrics@latest
        with:
          filename: github-metrics.svg
          token: ${{ SECRETS.METRICS_TOKEN }} # গিটহাব টোকেন ব্যবহার করতে হবে

          # টার্মিনাল বা কমপ্যাক্ট স্টাইল বজায় রাখতে নিচের অপশনগুলো দিন
          base: header, activity, community, repositories
          plugin_lines: yes
          plugin_languages: yes
          plugin_languages_ignored: details, html # আপনার পছন্দমতো ভাষা বাদ বা রাখতে পারেন
          plugin_languages_limit: 8
          plugin_activity: yes
          plugin_activity_days: 14
          plugin_activity_filter: all

    ![](https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=3000&pause=1000&color=39FF14&center=false&vCenter=true&width=435&lines=Frontend+Developer;Learning+JavaScript+%26+React;Building+Web+Apps)


    [![Mehedi's GitHub stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=radical)](https://github.com/anuraghazra/github-readme-stats)

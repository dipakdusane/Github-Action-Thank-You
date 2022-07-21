Github-Action :A way of saying thank you!
===============================================================================
Say thank you when someone makes a new Pull Request on your repository!
===============================================================================
Getting Started
Create a Tenor API key and set it as a Secret on your GitHub repo

name: Thank You

on:
  pull_request:
    types: [opened]

jobs:
  thanks:
    runs-on: actions/checkout@v2
    steps: ./
      - uses:
        with:
          GITHUB_TOKEN: ${{secrets.GITHUB_TOKEN}}
          TENOR_TOKEN: ${{secrets.TENOR_TOKEN}}
          
          
===============================================================================          



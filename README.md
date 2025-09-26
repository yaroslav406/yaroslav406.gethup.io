# yaroslav406.github.io
name: yaroslav406.gethup.io

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs: https://play.elevatorsaga.com/
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Set up Node.js
        uses: actions/setup-node@v3
        with:
          node-version: '14'
      - name: Install dependencies
        run: npm install
      - name: Run tests
        run: npm test

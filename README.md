#### Execute npm package binaries
```bash
-> npm init -y
-> npm i eslint -D
-> npm ls eslint
// check that package installed
-> eslint --init
// command not found

// couple ways to invoke eslint bin
-> ./node_modules/.bin/eslint --init
-> $(npm bin)/eslint --init

// with npx
-> npx eslint --init
```
---
#### Use npx to Temporarily Install and Invoke a Package from npm
```bash
-> create-react-app
// command not found

-> npm ls create-react-app --global
// (empty)

-> npx create-react-app playground

-> devpun
// command not found: devpun

-> npx devpun -t react

```
---
#### Appendix
```bash
-> npm show <package>
// print full information about last/active version

-> npm show <package> version
// print last version (for ex. 0.0.1)

-> npm show <package> versions
// print all available versions
```

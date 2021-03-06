#### Execute npm package binaries
```bash
-> npm init -y
-> npm i eslint -D
-> npm ls eslint
# check that package installed
-> eslint --init
# command not found

# couple ways to invoke eslint bin
-> ./node_modules/.bin/eslint --init
-> $(npm bin)/eslint --init

# with npx
-> npx eslint --init
```
---
#### Use npx to Temporarily Install and Invoke a Package from npm
```bash
-> create-react-app
# command not found

-> npm ls create-react-app --global
# (empty)

-> npx create-react-app playground

-> devpun
# command not found: devpun

-> npx devpun -t react
# prints a joke

-> npx devpun -t react | npx cowsay -f vader
-> npx devpun -t react | npx cowsay -f vader | npx lolcatjs
```
---
#### Different node module versions with npx
```bash
-> npm v create-react-app version
# prints current active version in registry
# `v` is alias for `view` or `show` or `info`

-> npx create-react-app@next app-name

-> npx -p eslint@next -p eslint-config-google -c "eslint ./"
# `-p` or `--path` flag specifies packages to install and add to the running $PATH
# `-c` executes <line> as "command"
```
---
#### Execute code from remote github repository
```bash
-> npx <githubname>/<githubrepo>#<branch>
```
---
#### Execute code from gist
```bash
-> npx https://gist.github.com/lgmkr/3af70ada30fad4ce4f0e59d33591d994
npx: installed 1 in 3.672s
Hello world!
```
---
#### Run commands with different Node versions
```bash
-> npx -p node@8.2.1 -- node index.js
# executes index.js with node version 8.2.1
```
---
#### Appendix
```bash
-> npm show <package>
# prints full information about last/active version

-> npm show <package> version
# print last version (for ex. 0.0.1)

-> npm show <package> versions
# print all available versions
```

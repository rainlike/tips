Yarn
====

**helpful links**
* [homepage](https://yarnpkg.com/en/)
* [configs](https://yarnpkg.com/lang/en/docs/cli/config/)
* [dependencies types](https://yarnpkg.com/en/docs/dependency-types)
* [dependency versions](https://yarnpkg.com/en/docs/dependency-versions)

**globally install**
```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update && sudo apt install yarn
```

**Start new project**
```
yarn init
```

**Adding a global dependency**
```
yarn global add {package}[@{version|tag}]
```

**Adding a local dependency**
```
yarn add {package}[@{version|tag}]
```
_possible options_
```
--dev/-D - will install package in devDependencies section
--peer  - will install package in peerDependencies section
--optional - will install package in optionalDependencies section
```

**Upgrade dependency**
```
yarn upgrade {package}[@{version|tag}]
```
_useful option_
```
--latest - upgrades packages, but ignores the version range specified in package.json
```

**Remove dependency**
```
yarn remove {package}
```

**Link to global package**
```
yarn link {package}
```

**Installing all dependencies of project**
```
yarn [install]
```
_useful options_
```
--flat - nstalling one and only one version of a package
--force - forcing a re-download of all packages
--production - installing only production dependencies
```

**View configs**
```
yarn config list
```

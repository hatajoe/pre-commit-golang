# pre-commit-golang
Golang pre-commit hooks for http://pre-commit.com/
## install
you need first to install (pre-commit) [https://pre-commit.com/#install]
```
brew install pre-commit
# to install pre-commit into your git hooks
pre-commit install
```
## Usage
Add a file named `.pre-commit-config.yaml` into the root directory of your repository 
```yaml
repos:
  - repo: git://github.com/Bahjat/pre-commit-golang
    rev: master
    hooks:
      - id: go-fmt-import
      - id: go-vet
      - id: go-lint
      - id: go-unit-tests
``` 
## Contributing
- Fork it
- Create your feature branch `git checkout -b my-new-feature`
- Commit your changes `git commit -am 'Add some feature'`
- Push to the branch `git push origin my-new-feature`
- Create new Pull Request

## Credits
This repo is inspired by [dnephin/pre-commit-golang](https://github.com/dnephin/pre-commit-golang)

## Finally
If you like this hooks please give a star
# Minimal requirements for applications

For any application, a minimal requirements should be follow as technical structure and organisation.

## Structure
- Any application has to be Dockeurise and deployable anywhere
- Any terms and specifications have to be templetized
- Any configurations and specifications have to be externalized

## Features
- Each features as possible as it can, have to be independant and be removable without breaking another one (of the same application)

## Documentation
☑️ Those points are not applicable for prototype
- Every project has to have a `README.md` explaining what the project is for
- Every project has to be fully documentized about its features and how does it work
- Every project has to have a notice explaining how deploying it in local from source as from Docker
- Every project has to have a notice explaining the code structure

## Quality
- Any code has to be Units tested with `>=80%` (as possible as it can)
- Any code has to be lint (using a standart tools)
- Any code has to be format (using a standart tools)
- Any json, yaml, toml, ... has to be lint (using a standart tools like [jq](https://stedolan.github.io/jq/) for example)
- Any units tests, linter, formatter, ... have to be easily run locally using hooks (like [tox](https://tox.wiki/en/latest/) or [pre-commit](https://pre-commit.com/) for example)

## Account and connexion
- No specifique account for individual (except admin and **one** basic user)
- Every connexion has to use the [ESN Galaxy](https://accounts.esn.org/) SSO

## CI/CD
- The CI/CD used has to be the [GitHub Actions](https://github.com/features/actions)
- The build has to be automatically launch on project tag using CI/CD
- Units tests, linter, quality, ... have to be automatically launch on push for any branch
- You are free to add any Workflows as you want

## Branchs
- No push into master
- 1 feature = 1 issue = 1 branch = 1 merge request
- No code if no issue attached
- Merge requests as possible as it can, have to be approuval by someone else
- No merge before any GitHub action passed

## Deployement
- Every deployement has to be as code from the repository [apps-as-code](https://github.com/ESNFranceG33kTeam/apps-as-code)



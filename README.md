<p align="center">
  <a href="https://github.com/jmatsu/dg-upload-app-action/actions"><img alt="typescript-action status" src="https://github.com/jmatsu/dg-upload-app-action/workflows/build-test/badge.svg"></a>
</p>

# Upload an app to DeployGate

This action uploads an application file to DeployGate. (Not official action of DeployGate.)

NOTE: `v0.2` does not have a backward compatibility with `v0.1`.

## Versions

See [Releases](https://github.com/jmatsu/dg-upload-app-action/releases) page.

## Inputs and Outpus

See *action.yml* of your version.

## Example

Please make sure your workflow will run when a branch is pushed.

```yaml
on:
  push or pull_request
```

Add this action to steps.

```yaml
uses: jmatsu/dg-upload-app-action@<version>
  with:
    app_owner_name: <your DeployGate account/organization name>
    api_token: ${{ secrets.DEPLOYGATE_API_TOKEN }} # for example
    app_file_path: /path/to/app_file
```

NOTE: [versioning documentation](https://github.com/actions/toolkit/blob/master/docs/action-versioning.md)

## License

[MIT License](LICENSE)

- [actions/typescript-action's LICENSE](https://github.com/actions/typescript-action/blob/master/LICENSE) (GitHub, Inc. and contributors) - this project uses the template from [actions/typescript-action](https://github.com/actions/typescript-action)

## Release

run [Release Drafter](./actions/workflows/release-drafter.yml)

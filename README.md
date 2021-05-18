# terraform-cli

This role enables to install terraform on a system.

## Requirements

No requirements.

## Role Variables

| Name                                 | Type   | Location            | Description                                                                             |
| ------------------------------------ | ------ | ------------------- | --------------------------------------------------------------------------------------- |
| terraform_version                    | string | `defaults/main.yml` | The version of terraform to install. Defaults to `0.15.3`.                              |
| terraform_releases_url               | string | `defaults/main.yml` | The base URL of terraform releases repository. Defaults to `https://releases.hashicorp.com/terraform`. |
| terraform_os                         | string | `defaults/main.yml` | The OS distribution of terraform to install. Defaults to `linux`.                       |
| terraform_arch                       | string | `defaults/main.yml` | The arch distribution of terraform to install. Defaults to `amd64`.                     |
| terraform_executable_sha256_checksum | string | `defaults/main.yml` | The expected checksum of the terraform executable downloaded from the website.          |

## Dependencies

No dependencies.

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  roles:
    - { role: julb.terraform_cli }
```

## License

MIT

## Author Information

More to find on my [Github](https://github.com/julb).

## Contributing

This project is totally open source and contributors are welcome.

When you submit a PR, please ensure that the syntax has been checked.

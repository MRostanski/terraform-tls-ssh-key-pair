
## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|:----:|:-----:|:-----:|
| attributes | Additional attributes (e.g. `1`) | list | `<list>` | no |
| chmod_command | Template of the command executed on the private key file | string | `chmod 600 %v` | no |
| delimiter | Delimiter to be used between `namespace`, `stage`, `name` and `attributes` | string | `-` | no |
| name | Application or solution name (e.g. `app`) | string | - | yes |
| namespace | Namespace (e.g. `cp` or `cloudposse`) | string | - | yes |
| private_key_extension | Private key extension | string | `` | no |
| public_key_extension | Public key extension | string | `.pub` | no |
| ssh_key_algorithm | SSH key algorithm | string | `RSA` | no |
| ssh_key_bits | SSH RSA key bits | string | `2048` | no |
| ssh_key_curve | SSH ECDSA elliptic curve | string | `P256` | no |
| ssh_public_key_path | Path to SSH public key directory (e.g. `/secrets`) | string | - | yes |
| stage | Stage (e.g. `prod`, `dev`, `staging`) | string | - | yes |
| tags | Additional tags (e.g. map(`BusinessUnit`,`XYZ`) | map | `<map>` | no |

## Outputs

| Name | Description |
|------|-------------|
| key_name | Name of SSH key |
| public_key | Contents of the generated public key |


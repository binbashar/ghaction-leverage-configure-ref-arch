# Github Action: Binbash Leverage - Reference Architecture

Set the Binbash Leverage Reference Architecture configuration files.

## Usage

Example:

```yaml
    - name: Configure Reference Architecture
      uses: binbashar/ghaction-leverage-configure-ref-arch@v0.4.1
      with:
        dir_name: "."
        project: "bb"
        project_long: "binbash"
        region_primary: "us-east-1"
        region_secondary: "us-east-2"
        aws_root_account_id: "${{ secrets.AWS_ROOT_ACCOUNT_ID }}"
        aws_security_account_id: "${{ secrets.AWS_SECURITY_ACCOUNT_ID }}"
        aws_shared_account_id: "${{ secrets.AWS_SHARED_ACCOUNT_ID }}"
        aws_devstg_account_id: "${{ secrets.AWS_DEVSTG_ACCOUNT_ID }}"
        aws_network_account_id: "${{ secrets.AWS_NETWORK_ACCOUNT_ID }}"
        vault_address: ""
        vault_token: ""
        sso_enabled: false
        sso_start_url: ""
        sso_region: ""
        toolbox_version: "1.2.7-0.1.2"
```

This is how the action is called.

All the secrets must be set prior to run this.

# Ansible Role: wkhtmltopdf

An Ansible Role that installs wkhtmltopdf on RedHat/CentOS, Debian and Ubuntu.

## Requirements

None

## Installation

`ansible-galaxy install vdzhorov.wkhtmltopdf`

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

    wkhtmltopdf_version: "0.12.6-1"

The version to use when installing `wkhtmltopdf`. See https://wkhtmltopdf.org/downloads.html for list of available versions.

    wkhtmltopdf_download_dest: "/usr/local/src"

The destination where `wkhtmltopdf` will be downloaded for installation.
    
    wkhtmltopdf_base_download_url: "https://github.com/wkhtmltopdf/packaging/releases/download"

The url from which `wkhtmltopdf` will be downloaded.

## Dependencies

None

## Example Playbook

    - hosts: wkhtmltopdf
      roles:
        - vdzhorov.wkhtmltopdf

## License

MIT

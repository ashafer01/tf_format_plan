# Terraform format_plan

This is a small script that formats ugly JSON blobs in plan outputs.

You can pipe the output of `terraform plan` or `terraform show <plan file>`
into this script, and any attribute changes containing JSON blobs will be
put side-by-side, and the JSON blobs will be pretty printed.

At present the script will do a simple truncation to your terminal width.

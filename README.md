# S3 Backups

This role runs a script on a timer that will sync a list of folders to an S3 bucket

## Requirements

Nothing unusual

## Role Variables

See `defaults/main.yml` for a full list of variables.

## Dependencies

None

## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
        - role: s3-backups
          schedule: daily
          bucket: foo-backups-bucket
          folders:
            - /path/to/a/folder
            - /path/to/another/folder
          exclusions:
            - /path/to/a/folder/exclude/this
          storage_class: GLACIER

## License

MIT

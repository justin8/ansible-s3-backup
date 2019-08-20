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
          s3_backup_schedule: daily
          s3_backup_bucket: foo-backups-bucket
          s3_backup_folders:
            - /path/to/a/folder
            - /path/to/another/folder
          s3_backup_exclusions:
            - /path/to/a/folder/exclude/this
          s3_backup_storage_class: GLACIER

## License

MIT

# humanics

## Docker

1. Get GitHub personal access token, than login to the registry:

  ```sh
  docker login ghcr.io -u alexkravets --password GITHUB_ACCESS_TOKEN
  ```

2. Update `/etc/hosts` file to add support for virtual domains by adding or
extending `127.0.0.1` line with:

  ```
  127.0.0.1 accounts.humanics.local instance.humanics.local
  ```

3. Create Docker stack:

  ```sh
  docker-compose up
  ```

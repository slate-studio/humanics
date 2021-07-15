# humanics

## Docker

1. Get GitHub personal access token, than login to the registry:

  ```sh
  export CR_PAT=GITHUB_ACCESS_TOKEN
  echo $CR_PAT | docker login ghcr.io -u alexkravets --password-stdin
  ```

2. Update `/etc/hosts` file to include virtual domains by replacing
`127.0.0.1 localhost` line with:

  ```
  127.0.0.1 localhost accounts.humanics.local instance.humanics.local
  ```

3. Create Docker stack:

```sh
docker-compose up
```

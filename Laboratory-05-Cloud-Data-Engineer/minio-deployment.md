# MinIO Deployment

## Deployment Command

The MinIO object storage server was deployed using Docker in the KillerCoda Ubuntu Playground. The following command was used:

```bash
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" quay.io/minio/minio server /data --console-address ":9001"
```

The `quay.io/minio/minio` image was used to deploy the MinIO server.

## Web Console Port

The MinIO Web Console was accessed through **port 9001**.

* **Port 9000** – MinIO API
* **Port 9001** – MinIO Web Console

The KillerCoda Traffic/Custom Ports feature was used to access port 9001 and open the MinIO Web Console.

## Bucket Created

A bucket named **client-photos** was created through the MinIO Web Console.

A sample file was then uploaded to the `client-photos` bucket to verify that object storage was working correctly.

## Environment Variables

The `-e` flags in the Docker command were used to define environment variables for the MinIO server.

The first environment variable:

```bash
-e "MINIO_ROOT_USER=cloudadmin"
```

sets the administrator username to `cloudadmin`.

The second environment variable:

```bash
-e "MINIO_ROOT_PASSWORD=CloudNova2026!"
```

sets the administrator password used to log in to the MinIO Web Console.

These environment variables configure the login credentials when the MinIO server starts.

## Verification

The command below was used to verify that the MinIO container was running:

```bash
docker ps
```

The `minio-server` container was displayed with an active status and ports 9000 and 9001 mapped.

## Screenshots

The deployment and bucket upload screenshots are stored in the `screenshots` folder:

* `minio-deployed.png`
* `minio-bucket-upload.png`


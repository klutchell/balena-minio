# balena-minio

[MinIO](https://min.io/) is a High Performance Object Storage released under Apache License v2.0. It is API compatible with Amazon S3 cloud storage service. Use MinIO to build high performance infrastructure for machine learning, analytics and application data workloads.

## Hardware Required

- Intel-NUC w/ +2GB RAM +128GB SSD

## Getting Started

You can one-click-deploy this project to balena using the button below:

[![Deploy with balena](https://balena.io/deploy.svg)](https://dashboard.balena-cloud.com/deploy?repoUrl=https://github.com/klutchell/balena-minio&defaultDeviceType=intel-nuc)

## Manual Deployment

Alternatively, deployment can be carried out by manually creating a [balenaCloud account](https://dashboard.balena-cloud.com) and application,
flashing a device, downloading the project and pushing it via the [balena CLI](https://github.com/balena-io/balena-cli).

### Environment Variables

| Name                  | Description                                                          |
| --------------------- | -------------------------------------------------------------------- |
| `MINIO_ROOT_USER`     | The access key for the root user. Defaults to `minioadmin` if unset. |
| `MINIO_ROOT_PASSWORD` | The secret key for the root user. Defaults to `minioadmin` if unset. |

<https://docs.min.io/minio/baremetal/reference/minio-server/minio-server.html#environment-variables>

## Usage/Examples

Once your device joins the fleet you'll need to allow some time for it to download the application and start the services.

When it's done you should be able to access the access the app at <http://minio.local>.

The default credentails are `minioadmin/minioadmin` and you should change them immediately via Environment Variables.

Additional usage instructions for MinIO can be found here: <https://docs.min.io/docs/minio-quickstart-guide.html>.

## Contributing

Please open an issue or submit a pull request with any features, fixes, or changes.

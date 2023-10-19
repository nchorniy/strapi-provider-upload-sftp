# strapi-provider-upload-sftp-v3

SFTP provider for Strapi CMS file upload - added support of Node 18.

## Installation

```
yarn add strapi-provider-upload-sftp-v3
```

## Config

`./extensions/upload/config/settings.json`

```json
{
  "provider": "sftp",
  "providerOptions": {
    "host": "<host>",
    "port": "<port>",
    "user": "<sftp-username>",
    "password": "<password>",
    "basePath": "<base-path>",
    "baseUrl": "<base-url>"
  }
}
```

## Base URL
`Base URL` is used to generate the URLs for the files. The file name will be appended to it.

Obs: the value should include a / at the end

### Example
```
Base URL: http://example.com/
File name: image.jpg

File URL: http://example.com/image.jpg
```

## Base PATH
`Base PATH` is used to define where, inside FTP, files should be saved.

## License

MIT License

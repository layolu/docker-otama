# docker-otama

[Otama][1] is a [CBIR][2] (Content-based image retrieval) engine.
It enables querying similar images database by an image file, and calculate the similarity between two images, and so on.

For the further details, please visit the project's [wiki page][3] on GitHub (Japanese).
(notice: I'm not the developer of Otama.)

## About this image
This image based on the debian:jassie image.

Otama in this image is built with following options:
- Enable MySQL Support for database
- Enable Leveldb (default)
- Install [ruby API][4] (default)

This image contains [example RPC server][5] in /opt/otamarpc directory, and run the server by default (CMD).

The setting file path of the server is /opt/otamarpc/config.yaml, so replace it with yours. 

[Utility commands][6] are also included.

[1]: https://github.com/nagadomi/otama
[2]: https://en.wikipedia.org/wiki/Content-based_image_retrieval
[3]: https://github.com/nagadomi/otama/wiki
[4]: https://github.com/nagadomi/otama/wiki/Ruby-API
[5]: https://github.com/nagadomi/otama/wiki/example-RPC
[6]: https://github.com/nagadomi/otama/wiki/Utility-commands

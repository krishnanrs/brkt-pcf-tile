# brkt-pcf-tile

A sample Bracket tile using the PCF tile generator (https://github.com/cf-platform-eng/tile-generator).

Use the PCF Tile Generator documentation to initialize your tile generator environment.

All required resources are available under the sample directory including a Bracket
Encryptor BOSH package which launches and run brkt-cli.

This tile:
 - Fetches a PCF stemcell from a specified URL
 - Encrypts the stemcell image in a specified region
 - Re-packages the stemcell and uploads it to a configured S3 bucket

The Bracket encryption (CLI) job runs as an errand within the tile.

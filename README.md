# Filebeat installer merge module for GPII

This produces `filebeat.msm`, which is used by gpii-wix-installer to bundle filebeat with the GPII. This will make the
GPII installer install and start the filebeat service.

## Usage

* Copy [filebeat-template.yml](filebeat-template.yml) into [filebeat/](filebeat/)filebeat.yml
* Add the elastic search credentials into the new file in the appropriate place.
* Run [build.bat](build.bat)
* Take `output/filebeat.msm`.

Don't commit `filebeat.yml` or `filebeat.msm`, because they contain credentials.

# buld_site_creator

Simple script to bulk create sites in the mist dashboard from CSV file.

## Prerequisits:

- config.py should have the `google_api_key` value filled out.
- google_api_key should have the google maps `Geocoding` and `Timezone` APIs allowed
  - This should be set as a local envirmental variable of GOOLE_API_KEY
    - MAC = export [variable_name]=[variable_value]
    - Windows = set [variable_name]=[variable_valuie]
- CSV with the following fields `site_name`, `site_address` with option fields `rf_template_name` and/or `spoke_template_name` and/or `network_template_name`

## Usage:

```bash
python ./site_creator.py -k <Mist API Key> -o <Mist Org ID>
```

### Update November 2022

Added the ability to push wan edge and network templates as part of the CSV - Fry

This is a fork of the Jake Synder's script that can be found at:

https://github.com/jsnyder-juniper/bulk_site_creator

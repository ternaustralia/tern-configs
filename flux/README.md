1. flux_data_publication_ozflux_dag.json
- this is the site config file for flux publication DAG for ozflux project
- Each site configuration is as below:
{
    "<sitename>": {
        "site_folder": <site staging foldername>,
        "alias": <site_name from the global variable of the netcdf file>,
        "parent_metadata_uuid": <UUID of the parent SHAReD metadata record of flux data collection>,
        "towers": [
            {
                "uri": <tower persistent identifier>,
                "file_prefixes": <List of netcdf file prefixes associated with the tower>
            }
        ]
    }
}
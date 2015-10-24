# System Module Format
---
All modules are contained in a directory with the following structure

    <module_dir>/<module_name>.json
                 <module_name>.json.hash
                 <module_name>.pl
                 @code/<module_name>__CONSTANTS.pl
                       <module_name>__INTERFACE.pl
                       <module_name>__CLASS.pl
                       <module_name>__EXTENSIONS.pl
                       <module_name>__ACTIONS.pl
                 @data/<module_name>__INIT_DATA.json
                       <module_name>__DATA.json
                 @docs/<module_name>__DOCS.txt
                 @_ccode_/<module_name>.exec


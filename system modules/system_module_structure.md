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

---
* `<module_name>`.json
    * This file has a JSON structure with information about the module and its components

* <module_name>.json.hash
    * This file has the HASH value (either a MD5 or a SHA1 hash) calculated from the <module_name>.json file

* <module_name>.<extension> (either .pl, .php, .py, etc)
    * This is the main code file to be called for the module initialization / loading

* @code  (directory)
    * This directory has the code files for the several sections of the module (both 'required' and 'optional' ones)

        * <module_name>__CONSTANTS.<extension>  (either .pl, .php, .py, etc)
            * This file has the definition of CONSTANTS for the module

        * <module_name>__INTERFACE.<extension>  (either .pl, .php, .py, etc)
            * This file has the definition of the public INTERFACE for the module (whenever it applicable)

        * <module_name>__CLASS.<extension>  (either .pl, .php, .py, etc)
            * This file has the definition of the CLASS or PACKAGE that implements the module

        * <module_name>__EXTENSIONS.<extension>  (either .pl, .php, .py, etc)
            * This file has the definition of the code to load EXTENSION modules dependente from this module

        * <module_name>__ACTIONS.<extension>  (either .pl, .php, .py, etc)
            * This file has the code for any necessary ACTIONS for the module

* @data  (directory)
    * This directory has the data files for the module

        * <module_name>__INIT_DATA.json
            *  This JSON file has the module's INITIAL DATA

        * <module_name>__DATA.json
            * This JSON file has the modules static DATA

* @docs  (directory)
     * This directory has the modules documentation

# `<module_name>`.json file
---
This file defines and controls the elements that make-up a module

It is a JSON format file

    code_loader.json
    {
        "name" : "code_loader" ,
        "version" : "5.0.000" ,
        "meta_base_dir" : "%%%__FILE___%%%" ,
        "base_dir" : "code_loader" ,
        "timestamp" : `<time-stamp>` ,
        "content":
        {
            "init_file" : "code_loader.pl" ,
            "descr_file" : "code_loader.json" ,
            "description" : "This is the code_loader module, in PERL implementation" ,
            "code" :
            {
                "dir" : "@code" ,
                "nr_comp" : 5 ,
                "components" :
                {
                    "CONSTANTS" :
                    {
                        "file_name" : "code_loader__CONMSTANTS.pl" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@code[@dir]]]}" ,
                        "file_path" : "code_loader/@code/" ,
                        "load_type" : "required"
                    } ,
                    "INTERFACE" :
                    {
                        "file_name" : "code_loader__INTERFACE.pl" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@code[@dir]]]}" ,
                        "file_path" : "code_loader/@code/" ,
                        "load_type" : "required"
                    } ,
                    "CLASS" :
                    {
                        "file_name" : "code_loader__CLASS.pl" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@code[@dir]]]}" ,
                        "file_path" : "code_loader/@code/" ,
                        "load_type" : "required"
                    } ,
                    "EXTENSIONS" :
                    {
                        "file_name" : "code_loader__EXTENSIONS.pl" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@code[@dir]]]}" ,
                        "file_path" : "code_loader/@code/" ,
                        "load_type" : "optional"
                    } ,
                    "ACTIONS" :
                    {
                        "file_name" : "code_loader__ACTIONS.pl" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@code[@dir]]]}" ,
                        "file_path" : "code_loader/@code/" ,
                        "load_type" : "optional"
                    }
                }
            } ,
            "data" :
            {
                "dir" : "@data" ,
                "nr_comp" : 3 ,
                "components" :
                {
                    "INIT_DATA" :
                    {
                        "file_name" : "code_loader__INIT_DATA.json" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@data[@dir]]]}" ,
                        "file_path" : "code_loader/@data/" ,
                        "load_type" : "required" ,
                        "data_format" : "text/json"
                    } ,
                    "STATIC_DATA" :
                    {
                        "file_name" : "code_loader__STATIC_DATA.json" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@data[@dir]]]}" ,
                        "file_path" : "code_loader/@data/" ,
                        "load_type" : "required" ,
                        "data_format" : "text/json"
                    } ,
                    "DATA" :
                    {
                        "file_name" : "code_loader__DATA.json" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@data[@dir]]]}" ,
                        "file_path" : "code_loader/@data/" ,
                        "load_type" : "required" ,
                        "data_format" : "text/json"
                    }
                }
            } ,
            "docs" :
            {
                "dir" : "@docs" ,
                "nr_comp" : 3 ,
                "components" :
                {
                    "DESCRIPTION" :
                    {
                        "file_name" : "code_loader__DESCRIPTION.txt" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@docs[@dir]]]}" ,
                        "file_path" : "code_loader/@docs/" ,
                        "load_type" : "optional"
                    } ,
                    "LICENSE" :
                    {
                        "file_name" : "code_loader__LICENSE.txt" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@docs[@dir]]]}" ,
                        "file_path" : "code_loader/@docs/" ,
                        "load_type" : "optional"
                    } ,
                    "META_DATA" :
                    {
                        "file_name" : "code_loader__META_DATA.txt" ,
                        "meta_path" : "{@base_dir}{__PATH_SEP__}{[@content[@docs[@dir]]]}" ,
                        "file_path" : "code_loader/@docs/" ,
                        "load_type" : "optional"
                    }
                }    
            } ,
            "code_cache" :
            {
                "dir" : "@_ccache" ,
                "nr_comp" : 1 ,
                "components" :
                {
                    "CODE_FILE" :
                    {
                        "file_name" : "code_loader.code.pl" ,
                        "meta_path" : null ,
                        "file_path" : "code_loader/@_ccache/" ,
                        "load_type" : "optional" ,
                        "rebuild" : false
                    } ,
                    "DEF_FILE" :
                    {
                        "file_name" : "code_loader.spec.json" ,
                        "meta_path" : null ,
                        "file_path" : "code_loader/@_ccache/" ,
                        "load_type" : "optional" ,
                        "rebuild" : false
                    }
            }
        }
    }

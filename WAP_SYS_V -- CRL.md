# WAP Sys V Common Runtime Layer


* IPL  (Initial Program Loader)
 * data_class
 * std_class
 * static_class
 * BESSAM (Back End Sub-System Access Manager)
 * sys_log
 * code_loader
 * core

* CRE  (Common Runtime Engine)
 * core
    * security
        * SAM  (Security Access Manager)
        * ACL   (Access Control Lists)
    * code_start
    * code_init
    * init
        * debug_logger
            * debug_logging
            * Log-1
            * Log-2
            *  ....
            * Log-n
        * code_runner
            * exception_handlers
                * ULS_exceptions
                * ULS_handlers
            * runtime_engine
                * code_interrupts
                * code_scheduler
                * code_threads
                * code_processes
                * code_interpreters
        * error_handler
            * bootstrap
                * app_args
                * p_state
                    * p_session
                        * base_static_class
                        * base data_class
                        * base_std_class
                * static_config
                * toolbox
                * app_engines
                    * app_engine_1
                    * app_engine_2
                    *   ....
                    * app_engine_n
                * arg_parser
            * boot_loader


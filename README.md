# APEXTranslationUK
Ukrainian Oracle Application Express translation

## Installation:

Using SQL*Plus login as your application's parsing schema and run script f4470_uk.sql passing your workspace name and your application id as parameters

Example:
    
    sqlplus /nolog
    connect username/password
    
    @f4470_uk.sql myworkspace 101

## Supported versions:
- [APEX 23.2](https://github.com/Oleh-Tyshchenko/APEXTranslationUK/archive/refs/tags/v23.2.zip)
- [APEX 23.1](https://github.com/Oleh-Tyshchenko/APEXTranslationUK/archive/refs/tags/v23.1.zip)


## Known issues:
- Long [**APEXIR_REMOVE_FLASHBACK**](/../../issues/9) (>29 symbols in UK) leads IR to fail with error *PL/SQL: numeric or value error: character string buffer too small*. If you face this issue edit the message using **Shared Components / Text Messages** and make it shorter.

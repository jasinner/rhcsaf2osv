# Red Hat CSAF to OSV Converter

## Setup

~~~
$ pipenv sync
$ pipenv shell
~~~

## Usage

Needs to be run in a folder where the Red Hat CSAF documents to convert already exist. Files can be downloaded the [Red Hat Customer Portal Security Data section](https://access.redhat.com/security/data/csaf/v2/advisories/)
~~~
$ ./csaf_converter.py csaf/rhsa-2024_4546.json
~~~

OSV documents will be output in the `osv` directory by default. Overwrite the default with the `--output_directory` option.

## Tests

~~~
$ python3 -m unittest rhel_osv/*_test.py
~~~
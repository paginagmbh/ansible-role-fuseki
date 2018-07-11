# Ansible Role: Apache Jena/Fuseki SPARQL Server

An Ansible Role that installs [Apache
Jena/Fuseki](https://jena.apache.org/documentation/fuseki2/) on Linux.

## Requirements

A Java runtime has to be installed on the target host.

## Example Playbook

``` yaml
- role: geerlingguy.java
- role: paginagmbh.fuseki
  fuseki_configurations:
    - name: "test-db"
      read_write: True
      union_default_graph: False
```

## License

BSD

## Author Information

This role was created in 2018 by [Pagina GmbH](https://www.pagina.gmbh/).
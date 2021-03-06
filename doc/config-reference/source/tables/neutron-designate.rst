..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _neutron-designate:

.. list-table:: Description of designate configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[designate]**
     -
   * - ``admin_auth_url`` = ``None``
     - (String) Authorization URL for connecting to designate in admin context
   * - ``admin_password`` = ``None``
     - (String) Password for connecting to designate in admin context
   * - ``admin_tenant_id`` = ``None``
     - (String) Tenant id for connecting to designate in admin context
   * - ``admin_tenant_name`` = ``None``
     - (String) Tenant name for connecting to designate in admin context
   * - ``admin_username`` = ``None``
     - (String) Username for connecting to designate in admin context
   * - ``allow_reverse_dns_lookup`` = ``True``
     - (Boolean) Allow the creation of PTR records
   * - ``ipv4_ptr_zone_prefix_size`` = ``24``
     - (Integer) Number of bits in an ipv4 PTR zone that will be considered network prefix. It has to align to byte boundary. Minimum value is 8. Maximum value is 24. As a consequence, range of values is 8, 16 and 24
   * - ``ipv6_ptr_zone_prefix_size`` = ``120``
     - (Integer) Number of bits in an ipv6 PTR zone that will be considered network prefix. It has to align to nyble boundary. Minimum value is 4. Maximum value is 124. As a consequence, range of values is 4, 8, 12, 16,..., 124
   * - ``ptr_zone_email`` =
     - (String) The email address to be used when creating PTR zones. If not specified, the email address will be admin@<dns_domain>
   * - ``url`` = ``None``
     - (String) URL for connecting to designate

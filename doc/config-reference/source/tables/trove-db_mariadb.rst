..
    Warning: Do not edit this file. It is automatically generated from the
    software project's code and your changes will be overwritten.

    The tool to generate this file lives in openstack-doc-tools repository.

    Please make any changes needed in the code, then run the
    autogenerate-config-doc tool from the openstack-doc-tools repository, or
    ask for help on the documentation mailing list, IRC channel or meeting.

.. _trove-db_mariadb:

.. list-table:: Description of MariaDB database configuration options
   :header-rows: 1
   :class: config-ref-table

   * - Configuration option = Default value
     - Description
   * - **[mariadb]**
     -
   * - ``api_strategy`` = ``trove.common.strategies.cluster.experimental.galera_common.api.GaleraCommonAPIStrategy``
     - (String) Class that implements datastore-specific API logic.
   * - ``backup_incremental_strategy`` = ``{'MariaDBInnoBackupEx': 'MariaDBInnoBackupExIncremental'}``
     - (Dict) Incremental Backup Runner based on the default strategy. For strategies that do not implement an incremental backup, the runner will use the default full backup.
   * - ``backup_namespace`` = ``trove.guestagent.strategies.backup.experimental.mariadb_impl``
     - (String) Namespace to load backup strategies from.
   * - ``backup_strategy`` = ``MariaDBInnoBackupEx``
     - (String) Default strategy to perform backups.
   * - ``cluster_support`` = ``True``
     - (Boolean) Enable clusters to be created and managed.
   * - ``default_password_length`` = ``${mysql.default_password_length}``
     - (Integer) Character length of generated passwords.
   * - ``device_path`` = ``/dev/vdb``
     - (String) Device path for volume if volume support is enabled.
   * - ``guest_log_exposed_logs`` = ``general,slow_query``
     - (String) List of Guest Logs to expose for publishing.
   * - ``guest_log_long_query_time`` = ``1000``
     - (Integer) The time in milliseconds that a statement must take in in order to be logged in the slow_query log.
   * - ``guestagent_strategy`` = ``trove.common.strategies.cluster.experimental.galera_common.guestagent.GaleraCommonGuestAgentStrategy``
     - (String) Class that implements datastore-specific Guest Agent API logic.
   * - ``icmp`` = ``False``
     - (Boolean) Whether to permit ICMP.
   * - ``ignore_dbs`` = ``mysql, information_schema, performance_schema``
     - (List) Databases to exclude when listing databases.
   * - ``ignore_users`` = ``os_admin, root``
     - (List) Users to exclude when listing users.
   * - ``min_cluster_member_count`` = ``3``
     - (Integer) Minimum number of members in MariaDB cluster.
   * - ``mount_point`` = ``/var/lib/mysql``
     - (String) Filesystem path for mounting volumes if volume support is enabled.
   * - ``replication_namespace`` = ``trove.guestagent.strategies.replication.experimental.mariadb_gtid``
     - (String) Namespace to load replication strategies from.
   * - ``replication_strategy`` = ``MariaDBGTIDReplication``
     - (String) Default strategy for replication.
   * - ``restore_namespace`` = ``trove.guestagent.strategies.restore.experimental.mariadb_impl``
     - (String) Namespace to load restore strategies from.
   * - ``root_controller`` = ``trove.extensions.common.service.DefaultRootController``
     - (String) Root controller implementation for mysql.
   * - ``root_on_create`` = ``False``
     - (Boolean) Enable the automatic creation of the root user for the service during instance-create. The generated password for the root user is immediately returned in the response of instance-create as the 'password' field.
   * - ``taskmanager_strategy`` = ``trove.common.strategies.cluster.experimental.galera_common.taskmanager.GaleraCommonTaskManagerStrategy``
     - (String) Class that implements datastore-specific task manager logic.
   * - ``tcp_ports`` = ``3306, 4444, 4567, 4568``
     - (List) List of TCP ports and/or port ranges to open in the security group (only applicable if trove_security_groups_support is True).
   * - ``udp_ports`` =
     - (List) List of UDP ports and/or port ranges to open in the security group (only applicable if trove_security_groups_support is True).
   * - ``usage_timeout`` = ``400``
     - (Integer) Maximum time (in seconds) to wait for a Guest to become active.
   * - ``volume_support`` = ``True``
     - (Boolean) Whether to provision a Cinder volume for datadir.
